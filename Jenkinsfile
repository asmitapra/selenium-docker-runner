pipeline {
    // master executor should be set to 0
    agent any
    stages {
        stage('Run Test') {
            steps {
                //sh
                
                sh '''
                ls
                docker compose --version
                docker ps
                
                '''
            }
        }
        stage('Bring Grid Down') {
            steps {
                //sh
                sh '''
                docker-compose down
                '''
            }
        }
    }
}
