pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/Mahalakshmi-lk/devops-cicd-pipeline.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t mahalakshmi76/devops-app .'
            }
        }

        stage('Push Docker Image') {
            steps {
                sh 'docker push mahalakshmi76/devops-app'
            }
        }
    }
}
