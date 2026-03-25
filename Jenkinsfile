pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Srikar746/exper7.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t exper7-image .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run exper7-image'
            }
        }

    }
}
