pipeline {
    agent any

    environment {
        PATH = "C:\\Users\\AKASH\\AppData\\Local\\Programs\\Python\\Python310;C:\\Users\\AKASH\\AppData\\Local\\Programs\\Python\\Python310\\Scripts;${env.PATH}"
    }

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