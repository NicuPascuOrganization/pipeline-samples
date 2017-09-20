pipeline {
  agent any
  parameters {
    choice(name: 'BRANCH', description: 'Branch', choices: 'master\ndevelop')
    credentials(name: 'CREDENTIAL', description: 'Credential', credentialType: "Username with password", required: true)
  }
  stages {
    stage('Build') {
      steps {
        echo "BRANCH: ${params.BRANCH} \n CREDENTIAL: ${params.CREDENTIAL}"
      }
    }
  }
}
