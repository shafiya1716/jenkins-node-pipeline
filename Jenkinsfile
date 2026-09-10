pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building Docker image...'
                bat 'docker build -t jenkins-node-app .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Docker image...'
                bat 'docker run --rm jenkins-node-app'
            }
        }
    }
}
