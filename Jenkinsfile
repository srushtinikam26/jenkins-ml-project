pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                echo 'Code already in workspace'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Training') {
            steps {
                bat 'python train.py'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}