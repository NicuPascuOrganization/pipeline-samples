pipeline {
  agent {
    label '!master'
  }
  stages {
    stage('Some stage') {
      steps {
        echo 'SOME MAIN STAGE'
      }
    }
    stage('Some stage 2') {
      steps {
        echo 'SOME MAIN STAGE'
      }
    }
    stage('Some stage 3') {
      steps {
        echo 'SOME MAIN STAGE'
      }
    }
  }
  post {
    always {
      script {
        echo "THIS IS POST TRIGGER STAGE"
      }
      
      
    }
    
    success {
      script {
        echo "THIS IS SUCCESS"
      }
      
      
    }
    
  }
}