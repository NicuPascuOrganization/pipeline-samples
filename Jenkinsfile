pipeline {
  agent any
  stages {
    stage('Build Parameters') {
      steps {
        script {
          def response = input message: 'User input required',
          parameters: [choice(name: 'Tag on Docker Hub', choices: 'no\nyes', description: 'Choose "yes" if you want to deploy this build')]
        }
        
      }
    }
  }
}