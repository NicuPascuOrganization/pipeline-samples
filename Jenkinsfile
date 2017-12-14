pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo "Hello World!"
      }
    }
    stage('Downstream') {
      parallel {
        stage('Down Alpha')
          steps {
            build 'downstream1' 
          }
        }
        stage('Down Beta') {
          steps {
            build 'downstream2' 
          }
        }
      }
    }
  }
}
