pipeline {
    agent {
        docker {
            image 'python:3.12-slim'
        }
    }

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Run App') {
            steps {
                sh 'python app.py'
            }
        }
    }
}
