pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                bat 'docker build -t my-python-app .'
            }
        }
        stage('Run Docker Container') {
            steps {
                bat 'docker run -d --rm -p 8081:8080 --name my-python-app my-python-app'
            }
        }
    }
}

