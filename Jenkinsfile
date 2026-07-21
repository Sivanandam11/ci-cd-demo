pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'sudo docker build -t ci-cd-demo .'
            }
        }

        stage('Stop Old Container') {
            steps {
                sh 'sudo docker stop website || true'
                sh 'sudo docker rm website || true'
            }
        }

        stage('Deploy') {
            steps {
                sh 'sudo docker run -d --name website -p 80:80 ci-cd-demo'
            }
        }
    }
}
