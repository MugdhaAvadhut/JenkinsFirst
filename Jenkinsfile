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
                cleanWs()
                cd /var/lib/jenkins/workspace/Hello
                chmod +x 'Hello.sh'
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
