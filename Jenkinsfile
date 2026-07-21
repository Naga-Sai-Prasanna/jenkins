pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    environment {
        COURSE = "Jenkins"
    }
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                        echo "building" 
                        echo $COURSE  

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
                script{
                    sh """
                        echo "deploying"
                    """
                }
            }
        }
    }
    //postbuild always run --even pipeline success or fail it will run

    post {
        always {
            echo 'I will always say Hello again!'
        }
        success {
            echo "pipeline success"
        }
        failure {
            echo "pipeline failure"
        }
    
    
    }
}