pipeline {
    agent any

    tools {
        maven 'Maven'
        jdk 'Java17'
    }

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Kusmitha123-kuppala/STUDENT-MANAGEMENT-DEV.git'
            }
        }

        stage('Maven Build & Test') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t student-management-app .'
            }
        }

        stage('Docker Run') {
            steps {
                sh '''
                docker stop studentapp || true
                docker rm studentapp || true
                docker run -d --name studentapp -p 8080:8080 student-management-app
                '''
            }
        }
    }
}
