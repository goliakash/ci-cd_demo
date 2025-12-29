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
        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Printing the python app') {
            steps {
                sh 'python3 app.py'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t python-ci-cd-app:latest .'
            }
        }
    }
}
