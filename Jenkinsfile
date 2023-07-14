pipeline {
    agent any
    
    stages {
        stage('Build') {
            when {
                expression {
                      env.BRANCH_NAME == 'master' && CODE_CHANGES == true
                  }
            }
            steps {
                echo "building the application..."
            }
        }
        
        stage('Test') {
            when {
                expression {
                   env.BRANCH_NAME == 'dev'
                }
            }
            steps {
                echo "testing the application...."
            }
        }
        
        stage('Deploy') {
            
            steps {
                echo "Deploying the application...."
            }
        }
    }
}
