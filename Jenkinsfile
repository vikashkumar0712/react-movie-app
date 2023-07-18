@Library("test-library") _
pipeline {
    agent any
    
    stages {
        stage('Greeting') {
            steps {
                helloWorld()
                // sh 'npm install -f' // Install dependencies
                // sh 'npm run build' // Build the React application
            }
        }
        
        stage('Test') {
            steps {
                testStage()
               // sh 'npm test' // Run tests
               //  echo "Test passed."
            }
        }
        
        // stage('Deploy') {
        //     steps {
        //         sh 'npm start'
        //     }
        // }
    }
}
