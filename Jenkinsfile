pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps { 
                echo 'Build World'
            }
        }
    stage ('Test'){
            steps { 
                echo 'Test World'
            }
        }
    stage ('Deploy'){
            steps { 
                echo 'Deploy World'
            }
        }
    }
    post
    {
      always
      {
      emailext bod: 'summary', subject: 'Pipeline Status', to: 'lakshyasharmaqa@gmail.com'
             }
         }
     }
      
