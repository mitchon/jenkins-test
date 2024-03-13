pipeline {
    agent {
        node { label 'gradle' }
    }
    stages {
        stage('build') {
            agent {
                docker {
                    image 'gradle:latest'
                }
            }
            steps {
                sh "./gradlew --version"
            }
        }
    }
    environment {
        GRADLE_USER_HOME = "$WORKSPACE/.gradle"
    }
}
