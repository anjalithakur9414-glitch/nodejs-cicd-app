pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/anjalithakur9414-glitch/nodejs-cicd-app.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t nodejs-cicd-app .'
            }
        }

        stage('Stop Old Container') {
            steps {
                sh 'docker stop node-app || true'
                sh 'docker rm node-app || true'
            }
        }

        stage('Run New Container') {
            steps {
                sh 'docker run -d -p 3000:3000 --name node-app nodejs-cicd-app'
            }
        }
    }
}
