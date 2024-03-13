pipeline {
    agent {
        node { label 'gradle' }
    }
    stages {
        stage('prepare') {
            env.GRADLE_USER_HOME = "$WORKSPACE/.gradle"
        }
        stage('build') {
            steps {
                sh "./gradlew --version"
            }
        }
    }
    environment {
        GRADLE_USER_HOME = '/jenkins/.gradle'
    }
}
