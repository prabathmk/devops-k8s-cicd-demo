pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t prabathmkdocker/devops-demo:v1 .'
            }
        }
        stage('Push') {
            steps {
                sh 'docker push prabathmkdocker/devops-demo:v1'
            }
        }
        stage('Deploy') {
            steps {
                sh 'kubectl apply -f deployment.yaml'
                sh 'kubectl apply -f service.yaml'
            }
        }
    }
}
