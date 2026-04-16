pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\AKASH\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" -m pip install --upgrade pip'
                bat '"C:\\Users\\AKASH\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Run Model') {
            steps {
                bat '"C:\\Users\\AKASH\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" train.py'
            }
        }
    }
}