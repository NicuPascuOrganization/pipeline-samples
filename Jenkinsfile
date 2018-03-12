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
      script {
        def response = input message: 'Success - Do you want to undeploy UAT environment?'
      }
      
      
    }
    
  }
}