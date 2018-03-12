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
    failure {
      echo 'Failure'
      
    }
    
    success {
      echo 'Success'
      
    }
    
  }
}