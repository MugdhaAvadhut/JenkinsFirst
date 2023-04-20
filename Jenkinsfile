pipeline{
  agent{label ''}
  options{
    buildDiscarder(logRotator(numToKeepStr:'10'))
}
  stages {
    
    stage('Message'){
      steps{
          bash Hello.sh
      }
    }
    stage('Deployment status'){
      steps{
          echo "Success"
      }
    }
  }
}
