pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/suresh-soumya/java-cicd-pipeline.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t java-cicd-pipeline .'
            }
        }

        stage('Push to Docker Hub') {
            steps {
                echo 'Docker Hub push will be configured next.'
            }
        }

        stage('Deploy to EC2') {
            steps {
                echo 'EC2 SSH deployment will be configured next.'
            }
        }
    }
}