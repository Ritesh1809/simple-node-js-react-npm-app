pipeline {
    agent any

    tools {
        nodejs "NodeJS" // This is the name of the NodeJS installation in Jenkins
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
                sh 'npm start &'
            }
        }
    }
}

