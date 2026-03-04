pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Omgmmui/ci-cd-devops-project.git'
            }
        }

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