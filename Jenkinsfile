pipeline {
    // master executor should be set to 0
    agent any
    stages {
        stage('Run Test') {
            steps {
                //sh
                
                sh '''
                cd /tmp 
                docker-compose -f docker-compose.yaml up
                '''
            }
        }
        stage('Bring Grid Down') {
            steps {
                //sh
                sh '''
                cd /tmp 
                docker-compose -f docker-compose.yaml down
                '''
            }
        }
    }
}
