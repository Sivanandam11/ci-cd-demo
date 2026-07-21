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
                sh 'docker build -t ci-cd-demo .'
            }
        }

        stage('Stop Old Container') {
            steps {
                sh 'docker stop website || true'
                sh 'docker rm website || true'
            }
        }

        stage('Deploy Website') {
            steps {
                sh 'docker run -d --name website -p 80:80 ci-cd-demo'
            }
        }
    }
}
