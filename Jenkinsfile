pipeline {
  agent any
  stages {
    stage('Run Tests') {
      steps {
        bat 'exit 1'
      }
    }
    stage('Deploy') {
      parallel {
        stage('Dev') {
          when {
            branch 'master'
          }
          steps {
            echo 'hello master'
          }
        }
        stage('QA') {
          steps {
            echo 'hello stable'
          }
        }
      }
    }
  }
}