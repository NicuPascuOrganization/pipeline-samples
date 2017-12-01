pipeline {
  agent any
  stages {
    stage('One') {
      steps {
        retry(count: 5) {
          echo 'DDDDDD'
          echo 'EEEEEE'
          echo 'FFFFFF'
          timeout(time: 30) {
            echo 'ZZZZZZ'
          }
          
        }
        
        sh 'echo \'AAAAAA\'; ping -c 5 localhost'
        sh 'echo \'BBBBBB\'; ping -c 5 localhost'
        sh 'echo \'CCCCCC\'; ping -c 20 localhost'
      }
    }
    stage('Two') {
      steps {
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
      }
    }
    stage('Three') {
      steps {
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
      }
    }
    stage('Four') {
      steps {
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
      }
    }
    stage('Five') {
      steps {
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
        sh 'echo `date`; ping -c 5 localhost'
      }
    }
  }
}