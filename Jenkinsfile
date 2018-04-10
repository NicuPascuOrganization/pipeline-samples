pipeline {
  agent {
    node {
      label '}'
    }
    
  }
  stages {
    stage('Select version') {
      steps {
        script {
          input (message: "Select from the list", parameters: [choice(name: "version", choices: "0.1\n0.2\n0.3\n0.4\n0.5\n0.6\n0.7", description: "Version")])
        }
        
      }
    }
    stage('Deploy') {
      steps {
        script {
          println "Deploying..."
          sleep(10)
        }
        
      }
    }
    stage('Build Parameters') {
      steps {
        script {
          def response = input message: 'Do you want to\nundeploy UAT \n environment?'
        }
        
        script {
          input(message: 'User input required\nSecond line', ok: 'Engage!', parameters: [
            string(name: 'STRING', description: 'String Param\nSecond Line', defaultValue: 'Hello'),
            text(name: 'TEXT', description: 'Text Param', defaultValue: 'This is a\nmulti line string'),
            password(name: 'PASSWORD', description: 'Password Param', defaultValue: 'foo'),
            booleanParam(name: 'BOOLEAN', description: 'Boolean Param', defaultValue: false),
            choice(
              name: 'CHOICE',
              description: 'Choice Param',
              choices: 'master\ndevelop\nrelease-1.0\nrelease-2.0'
            )
          ])
        }
        
      }
    }
  }
}