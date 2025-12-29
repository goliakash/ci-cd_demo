pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                echo 'Code checked out successfully'
            }
        }

        stage('Check Workspace') {
            steps {
                sh 'pwd'
                sh 'ls'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t python-ci-cd-app:latest .'
            }
        }
    }
}
