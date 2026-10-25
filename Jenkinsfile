pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    environment {
        course = "Jenkins"  
    }
     options {
        disableConcurrentBuilds()
        timeout(time: 15, unit: 'MINUTES')
    }
    // Build
    stages {
        stage('Build') {
            steps {
               script {
                    echo 'Building..'
                    echo "Course name is ${course}"
                    sleep 5
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
