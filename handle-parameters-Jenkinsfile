pipeline {
  agent any
  parameters {
    string(name: 'Greeting', defaultValue: 'Hello', description: 'Some description')
  }
  stages {
    stage('Example') {
      steps {
        echo "${params.Greeting} World!"
      }
    }
  }
}