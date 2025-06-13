pipeline {
    agent any

    // Define custom environment variables
    environment {
        APP_VERSION = '1.0.3' // Example application version
        DEPLOY_ENV = 'staging' // Deployment environment
        AUTHOR_NAME = 'Faisal Ali' // Example author name
    }

    stages {
        stage('Build') {
            steps {
                echo "Building version: ${env.APP_VERSION}"
                echo "Author: ${env.AUTHOR_NAME}"
                // Your build logic here
            }
        }

        stage('Test') {
            steps {
                echo "Running tests for version: ${env.APP_VERSION}"
                // Your test logic here
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying version: ${env.APP_VERSION} to environment: ${env.DEPLOY_ENV}"
                // Your deployment logic here
            }
        }
    }
}
