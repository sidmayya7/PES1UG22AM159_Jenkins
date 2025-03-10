pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ hello.cpp -o PES1UG22AM159-1'
                echo 'Build Stage Successful'
            }
        }

        stage('Test') {
            steps {
                sh './PES1UG22AM159-1'
                echo 'Test Stage Successful'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful (Placeholder)'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
