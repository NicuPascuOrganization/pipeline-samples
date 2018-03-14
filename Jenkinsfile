pipeline {
  agent any
  stages {
    stage('Example') {
      steps {
        echo 'Hello World'
      }
    }
  }
  post {
    always {
      script {
        echo 'Hello World from post'
      }
      
      
    }
    
  }
}