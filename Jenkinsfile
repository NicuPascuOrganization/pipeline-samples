pipeline {
  agent any
  parameters {
    string(name: 'STRING1_NO_DESC')
    string(name: 'STRING2_WITH_DESC', description: 'With Description')
    string(name: 'STRING3_WITH_DEFAULT, description: 'String 3', defaultValue: 'Hello World')
  }
  stages {
    stage('Build') {
      steps {
        echo "Hello World!"
      }
    }
  }
}
