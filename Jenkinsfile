pipeline {
    agent any
    stages {
        stage("Checkout GitHub Repo") {
            steps {
                checkout scm
            }
        }
        stage('Npm install') {            
            steps {
                bat "npm install"
            }
        } 
        stage('Run tests') {            
            steps {
                bat "npm run test"
            }
        }                
    }
    // Post-build actions, notifications, etc.
}