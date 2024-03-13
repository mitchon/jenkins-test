pipeline {
    agent {
        node { label 'gradle' }
    }
    stages {
        agent {
            docker {
                image 'gradle:latest'
            }
        }
        stage('build') {
            steps {
                sh "./gradlew --version"
            }
        }
    }
    environment {
        GRADLE_USER_HOME = "$WORKSPACE/.gradle"
    }
}
