pipeline {
    agent {
        node { label 'gradle' }
    }
    stages {
        stage('build') {
            steps {
                sh './gradlew --version'
            }
        }
    }
    environment {
        GRADLE_USER_HOME = '/jenkins/.gradle'
    }
}
