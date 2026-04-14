pipeline {
    agent any

    stages {
        stage('Checkout Info') {
            steps {
                echo 'Pipeline started'
                sh 'whoami'
                sh 'hostname'
                sh 'pwd'
                sh 'ls -la'
            }
        }

        stage('Build') {
            steps {
                echo 'Running build stage'
                sh 'echo Build successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Running test stage'
                sh 'echo Tests successful'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished'
        }
        success {
            echo 'Pipeline succeeded'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
