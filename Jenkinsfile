pipeline {
    agent {
        docker {
            args '-v /jenkins/.gradle:/jenkins/.gradle'
            image 'gradle:latest'
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'gradle --version'
            }
        }
    }
    environment {
        GRADLE_USER_HOME = '/jenkins/.gradle'
    }
}