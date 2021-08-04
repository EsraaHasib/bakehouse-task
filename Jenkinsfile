pipeline {
    agent any
    stages {
        stage('Apply namespace') {
            steps {
                sh 'kubectl apply -f namespace.yaml'
            }
        }   
        stage('Apply Deployment') {
            steps {
                sh 'kubectl apply -f deployment.yaml'
            }
        }
        stage('Service') {
            steps {
                sh 'kubectl apply -f service.yaml'
            }
        }
    }
}