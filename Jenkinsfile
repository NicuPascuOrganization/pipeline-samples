pipeline {
  agent any
  stages {
    stage('Build Parameters') {
      steps {
        echo "params: $params"
        sh 'env'
      }
    }
  }
  parameters {
    choice(choices: '''CI
DEV
PROD''', description: 'Is this a DEV or a PROD build?', name: 'BUILD_TYPE')
    text(description: 'Release Notes (Type "t" to switch focus to search bar. "t" will always remove focus, making it impossible to type a full description.)', name: 'RELEASE_NOTES', defaultValue: 'CI Build')
  }
}