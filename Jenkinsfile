pipeline {
    agent {
        node { label 'gradle' }
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
