pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the specified SCM (configured in Jenkins)
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add your build commands or scripts here
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands or scripts here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add your deployment commands or scripts here
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }

        failure {
            echo 'Pipeline failed! Check the logs for more information.'
        }
    }
}
