pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'curl -sL https://deb.nodesource.com/setup_18.x | sudo -E bash -'
                sh 'sudo apt-get install -y nodejs'
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
            }
        }
    }
}
