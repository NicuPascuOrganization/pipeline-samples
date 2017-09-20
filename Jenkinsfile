pipeline {
  agent any
  stages {
    stage('Intro') {
      steps {
        echo "Hello World!"
      }
    }
    stage('Input') {
      steps {
        input(message: 'User input required', ok: 'Engage!',
          parameters: [
            string(name: 'STRING', description: 'String Param', defaultValue: 'Hello')
            text(name: 'TEXT', description: 'Text Param', defaultValue: 'This is a\nmulti line string')
            password(name: 'PASSWORD', description: 'Password Param', defaultValue: 'foo')
            booleanParam(name: 'BOOLEAN', description: 'Boolean Param', defaultValue: false)
            choice(
              name: 'CHOICE',
              description: 'Choice Param',
              choices: 'master\ndevelop\nrelease-1.0\nrelease-2.0'
            )
          ]
        )
      }
    }
    stage('Outro') {
      steps {
        echo "Goodbye World!"
      }
    }
  }
}
