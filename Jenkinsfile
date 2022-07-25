pipeline {
    agent any
    tools {
        gradle 'Gradle'
    }
    environment {
        NEW_VERSION = '1.3.0'
        GIT_CREDENTIALS = credentials('GIT_CREDS')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo "Building version ${NEW_VERSION}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo "Deploying.... ${NEW_VERSION}"
            }
        }
    }
}