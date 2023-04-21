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
            stage('Permission') {
            steps {
                sudo chmod 777 'Hello.sh'
                 }
            }
         stage('Script') {
            steps {
                sh 'Hello.sh'
                 }
            }
        stage('Deployment Complete'){
            steps{
                echo"Successfull"
                }
            }
        }
    }
