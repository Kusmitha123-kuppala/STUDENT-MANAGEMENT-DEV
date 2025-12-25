pipeline {
    agent any

    tools {
        jdk 'jdk17'
        maven 'maven3'
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
                bat 'mvn clean package'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t student-management-app .'
            }
        }

        stage('Docker Run') {
            steps {
                bat '''
                docker stop studentapp || exit 0
                docker rm studentapp || exit 0
                docker run -d --name studentapp -p 8080:8080 student-management-app
                '''
            }
        }
    }
}
