pipeline {
  agent any
  stages {
    stage('Build Parameters') {
      steps {
        script {
          def response = input message: 'Do you want to\nundeploy UAT \n environment?'
        }
        
        script {
          input(message: 'User input required\nSecond line', ok: 'Engage!', parameters: [
            string(name: 'STRING', description: 'String Param', defaultValue: 'Hello'),
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