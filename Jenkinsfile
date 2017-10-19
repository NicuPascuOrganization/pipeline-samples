pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello...'
        sleep 15
        echo '... World!'
        ws(dir: 'ws1') {
          echo 'hello workspace 1'
        }
        
        ws(dir: 'ws2') {
          echo 'hello workspace 2'
        }
        
        echo 'Finish'
      }
    }
  }
}