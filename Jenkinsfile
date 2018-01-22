pipeline {
  agent any
  stages {
    stage('Make a huge long string') {
      steps {
        sh 'for i in `seq 1 100`; do cat /dev/urandom | env LC_CTYPE=c tr -dc \\\'[:alpha:]\\\' | head -c 50000; done'
      }
    }
  }
  post {
    always {
      echo 'ALWAYS --> Runs all the time.'
      deleteDir()
      
    }
    
    success {
      echo 'SUCCESS --> Whatever we did, it worked. Yay!'
      
    }
    
    failure {
      echo 'FAILURE --> Failed. Womp womp.'
      
    }
    
  }
  options {
    buildDiscarder(logRotator(numToKeepStr: '20'))
  }
}