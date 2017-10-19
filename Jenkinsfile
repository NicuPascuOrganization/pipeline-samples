pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello...'
        sleep 300
        echo '... World!'
        ws(dir: 'workspacedir') {
          echo 'hello workspace'
        }
        
      }
    }
  }
}