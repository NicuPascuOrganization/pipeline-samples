pipeline {
  agent any
  stages {
    stage('One') {
      steps {
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
        retry(count: 5) {
          echo 'retry-a-1'
          echo 'retry-a-2'
          echo 'retry-a-3'
        }
        
      }
    }
    stage('Two') {
      steps {
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
      }
    }
    stage('Three') {
      steps {
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
      }
    }
    stage('Four') {
      steps {
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
      }
    }
    stage('Five') {
      steps {
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
        sh 'echo `date`; ping -c 20 localhost'
      }
    }
  }
}