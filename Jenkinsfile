pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    // Build
    stages {
        stage('Build') {
            steps {
               script {
                    echo 'Building..'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo 'Testing..'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying....'
                }
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success {
                echo 'I will run when it is successful!'
            }
        failure {
                echo 'I will run when it is failed!'
            }
    }
}
