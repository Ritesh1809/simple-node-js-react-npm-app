pipeline {
    agent { label 'local' }

    tools {
        nodejs "NodeJS" // Adjust this to your NodeJS installation name in Jenkins
    }

    environment {
        PORT = '3004' // Set the PORT environment variable
    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Serve') {
            steps {
                // Use 'nohup' to keep the server running in the background
                sh 'nohup npm start &'
            }
        }
    }
    
}


