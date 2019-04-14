pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh 'make check'
      }
    }
  }
  post {
    // always, changed, fixed, regression, aborted, failure, success, unstable, unsuccessful, cleanup
    always {
      junit '**/target/*.xml'
    }
    failure {
      mail to: misdu17@gmail.com, subject: 'The Pipeline failed...'
    }
  }
}