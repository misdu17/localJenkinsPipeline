pipeline {
    agent { docker { image 'maven:3.6.0-jdk-8-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
