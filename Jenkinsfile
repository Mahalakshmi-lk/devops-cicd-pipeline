pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/Mahalakshmi-lk/devops-cicd-pipeline.git'
            }
        }

        stage('Docker Login') {
            steps {
                sh 'docker login -u mahalakshmi76 -p YOUR_PASSWORD'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t mahalakshmi76/devops-app .'
            }
        }

        stage('Push to Docker Hub') {
            steps {
                sh 'docker push mahalakshmi76/devops-app'
            }
        }
    }
}
