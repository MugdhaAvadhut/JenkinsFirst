pipeline {
    agent none
    stages {
        stage('permission') {
            steps {
                chmod 777 Hello.sh
            }
            stage('build') {
            steps {
                sh Hello.sh
                }
            }
        }
    }
}
