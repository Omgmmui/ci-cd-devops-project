pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t letslearndevops2025/devops-app .'
            }
        }

        stage('Docker Login') {
            steps {
                bat 'docker login -u letslearndevops2025 -p Mohammed@7866'
            }
        }

        stage('Push Docker Image') {
            steps {
                bat 'docker push letslearndevops2025/devops-app:latest'
            }
        }

    }
}