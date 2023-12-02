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
        stage('Deploy') {            
            steps {
                withCredentials([usernamePassword(credentialsId: '7b91efe8-df57-4447-b6f6-64218c5a0b43', passwordVariable: 'password', usernameVariable: 'user')]) {
                    
                }
            }           
        }                      
    }
    
}