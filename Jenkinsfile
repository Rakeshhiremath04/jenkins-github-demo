pipeline {
    agent any

    environment {
        APP_NAME = 'MyDevOpsApplication'
        ENVIRONMENT = 'Development'
    }

    stages {
        stage('Build') {
            steps {
                echo "Building ${APP_NAME}"
                bat 'echo Build completed'
            }
        }

        stage('Test') {
            steps {
                echo "Testing ${APP_NAME}"
                bat 'echo Tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying to ${ENVIRONMENT}"
                bat 'echo Deployment completed'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed. Check the logs.'
        }

        always {
            echo 'Pipeline execution finished.'
        }
    }
}    
