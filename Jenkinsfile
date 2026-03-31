pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'YOUR_GITHUB_REPO_LINK'
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
