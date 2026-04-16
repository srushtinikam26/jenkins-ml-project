pipeline {
    agent any

    stages {
        stage('Check Python') {
            steps {
                bat 'where python'
                bat 'python --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Model') {
            steps {
                bat 'python train.py'
            }
        }
    }
}