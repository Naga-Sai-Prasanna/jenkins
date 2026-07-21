pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                        echo "building"
                    """
                }
            }
        }
        stage('Test') {
            steps {
                script{
                    sh """
                        echo "testing"
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "deploying"'
            }
        }
    }
}