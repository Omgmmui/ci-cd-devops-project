pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t letslearndevops2025/devops-app .'
            }
        }

        stage('Push Docker Image') {
            steps {
                bat 'docker push letslearndevops2025/devops-app:latest'
            }
        }

    }
}