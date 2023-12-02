pipeline {
    agent none
    stages {
        stage("Checkot github repo"){
            steps {      
                checkout scm          
                // script {
                //     checkout([$class: 'GitSCM',
                //               branches: [[name: 'master']],
                //               userRemoteConfigs: [[url: 'https://github.com/Sand82/Student-Registry-JenkinsFile.git']]]                              )
                // }
            }
        }
        stage('Npm install') {            
            steps{
                bat "npm install"
            }
        } 
        stage('Run tests') {            
            steps{
                bat "npm run test"
            }
        }                
    }
}
