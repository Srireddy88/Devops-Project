pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Srireddy88/Devops-Project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t devops-flask-app -f docker/Dockerfile .'
                }
            }
        }
    }
}
