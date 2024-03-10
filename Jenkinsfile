pipeline {
    agent {
        gradle
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
