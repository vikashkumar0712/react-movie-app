pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'npm install' // Install dependencies
                sh 'npm run build' // Build the React application
            }
        }
        
        stage('Test') {
            when {
                branch 'dev'
            }
            steps {
                sh 'npm test' // Run tests
            }
        }
        
        stage('Deploy') {
            steps {
                npm run install
                // Add your deployment steps here
            }
        }
    }
}
