pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo "Hello World!"
      }
    }
    stage('Downstream') {
      parallel(
        downstream1: {
          build 'downstream1' 
        },
        downstream2: {
          build 'downstream2' 
        }
      )
    }
  }
}
