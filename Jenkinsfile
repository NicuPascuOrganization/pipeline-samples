pipeline {
  agent any
  stages {
    stage('Build Parameters') {
      steps {
        script {
          def response = input message: 'Do you want to undeploy UAT environment?'
        }
        
      }
    }
  }
}