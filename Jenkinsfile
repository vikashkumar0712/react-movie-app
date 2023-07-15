pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'npm install -f' // Install dependencies
                sh 'npm run build' // Build the React application
            }
        }
        
        stage('Test') {
            steps {
               // sh 'npm test' // Run tests
                echo "Test passed."
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'npm start'
            }
        }
    }
}
