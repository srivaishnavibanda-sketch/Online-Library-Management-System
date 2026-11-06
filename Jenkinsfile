pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Downloading code from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building Online Library Management System'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Online Library Management System'
                bat 'dir'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }

    post {
        success {
            echo 'Pipeline Executed Successfully'
        }
        failure {
            echo 'Pipeline Failed'
        }
    }
}
