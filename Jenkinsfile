pipeline {
    agent any

    stages {

        stage('Check Files') {
            steps {
                sh 'pwd'
                sh 'ls -l'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t employee-management-portal:pipeline .'
            }
        }

        stage('Show Images') {
            steps {
                sh 'docker images'
            }
        }

    }
}
