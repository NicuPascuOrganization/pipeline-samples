pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        post() {
          always() {
            script {
              def response = input message: 'Do you want to undeploy UAT environment?'
            }
            
          }
          
        }
        
      }
    }
  }
}