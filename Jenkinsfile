pipeline {
    agent any
    stages {
        stage('Apply Deployment') {
            steps {
                sh 'kubectl apply -f deploymet.yaml'
            }
        }
        stage('Service') {
            steps {
                sh 'kubectl apply -f service.yaml'
            }
        }
    }
}