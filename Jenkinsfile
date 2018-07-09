pipeline {
  agent any
  stages {
    stage('One') {
      steps {
        sh 'echo `date`; ping -c 3 localhost'
        sh 'echo `date`; ping -c 3 localhost'
      }
    }
    stage('Two') {
      steps {
        sh 'echo `date`; ping -c 3 localhost'
      }
    }
    stage('Three') {
      steps {
        sh 'echo `date`; ping -c 3 localhost'
      }
    }
    stage('Four') {
      steps {
        sh 'echo `date`; ping -c 3 localhost'
      }
    }
    stage('Five') {
      steps {
        sh 'echo `date`; ping -c 3 localhost'
      }
    }
  }
}