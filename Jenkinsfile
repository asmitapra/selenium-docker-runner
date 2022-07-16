pipeline {
    // master executor should be set to 0
    agent any
    stages {
        stage('Run Test') {
            steps {
                //sh
                sh "sudo docker-compose up"
            }
        }
        stage('Bring Grid Down') {
            steps {
                //sh
                sh "sudo docker-compose down"
            }
        }
    }
}
