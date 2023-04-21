pipeline {
    agent {label ''}
    options {
        buildDiscarder(logRotator(numToKeepStr:'10'))
           }
        
    stages {
        
        stage('Message') {
            steps {
                echo "This is Jenkins"
            }
         }
         stage('Script') {
            steps {
                sh '/home/ubuntu/scripts/Hello.sh'
                 }
            }
        stage('Deployment Complete'){
            steps{
                echo"Successfull"
                }
            }
        }
    }
