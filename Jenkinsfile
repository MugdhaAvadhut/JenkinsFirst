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
                sh "chmod +x  ${env.WORKSPACE}"
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
