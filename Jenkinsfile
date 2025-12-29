pipeline {
    agent any

    stages {
        stage('Checkworkspace') {
            steps {
                sh 'pwd'
            }
        }
        stage('Run Python Script') {
            steps {
                sh 'python3 --version'
                sh 'python3 app.py'
            }
        }
    }
}
