pipeline{
  agent{label ''}
  options{
    buildDiscarder(logRotator(numToKeepStr:'10'))
}
  stages {
    
    stage('Message'){
      steps{
          echo "This is first pipeline"
      }
    }
    stage('Deployment status'){
      steps{
          echo "Success"
      }
    }
  }
}
