pipeline {
  agent any
  parameters {
    string(name: 'STRING1')
    string(name: 'STRING2', description: 'With Description')
    string(name: 'STRING3', description: 'With Default Value', defaultValue: 'Hello World')
  }
  stages {
    stage('Build') {
      steps {
        echo "STRING1: ${params.STRING1 \n STRING2: ${params.STRING2} \n STRING3: ${params.STRING3}"
      }
    }
  }
}
