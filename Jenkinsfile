pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-python-app .'
            }
        }
        stage('Run Docker Container') {
            steps {
                sh 'docker run -d --rm -p 8081:8080 --name my-python-app my-python-app'
            }
        }
    }
}
