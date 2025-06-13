pipeline {
    agent any

    environment {
        APP_VERSION = '1.0.3'        // Example application version
        DEPLOY_ENV = 'staging'       // Deployment environment
        AUTHOR_NAME = 'Anas Zeeshan' // Example author name
    }

    stages {
        stage('Build') {
            steps {
                echo "Building version: ${env.APP_VERSION}"
                echo "Author: ${env.AUTHOR_NAME}"
                // Use bat for Windows instead of sh
                bat 'echo Simulating build process...'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests for version: ${env.APP_VERSION}"
                bat 'echo Simulating test process...'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying version: ${env.APP_VERSION} to environment: ${env.DEPLOY_ENV}"
                bat 'echo Simulating deployment...'
            }
        }
    }
}
