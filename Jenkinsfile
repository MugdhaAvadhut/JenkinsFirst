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
                sh '/var/lib/jenkins/workspace/Hello/Hello.sh'
                 }
            }
        stage('Deployment Complete'){
            steps{
                echo"Successfull"
                }
            }
        }
    }
