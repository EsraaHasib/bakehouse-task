pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build . --tag esraahasib/cicd:v1'
            }
        }
        stage('Push') {
            steps {
                sh 'docker push esraahasib/cicd:v1'
            }
        }
    }
}