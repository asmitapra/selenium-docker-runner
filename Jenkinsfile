pipeline {
    // master executor should be set to 0
    agent any
    stages {
        stage('Run Test') {
            steps {
                //sh
                sh "docker-compose up"
            }
        }
        stage('Bring Grid Down') {
            steps {
                //sh
                sh "docker-compose down"
            }
        }
    }
}
