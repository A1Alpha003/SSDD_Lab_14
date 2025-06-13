pipeline {
    agent any

    tools {
        // Use the exact name of your Maven configuration
        maven 'Maven'
    }

    environment {
        // Define any environment variables you may need
        APP_VERSION = '1.0.3'
    }

    stages {
        stage('Setup') {
            steps {
                echo "Setting up environment for Maven..."
            }
        }

        stage('Build') {
            steps {
                // For Windows, use 'bat' instead of 'sh'
                bat 'mvn --version' // Verify Maven installation
                bat 'mvn clean install' // Install dependencies and build
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test' // Run tests using Maven
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application version ${env.APP_VERSION}..."
                // Add your deployment logic here
            }
        }
    }
}
