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
                sh 'docker build -t jenkins-demo:v1 .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm jenkins-demo:v1'
            }
        }
    }
}
