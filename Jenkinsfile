pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/brownm65/jenkins-node-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run App Check') {
            steps {
                sh 'node -v'
                sh 'npm -v'
            }
        }
    }
}