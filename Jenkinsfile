pipeline {
    agent any
    stages {
            stage('Git Checkout') {
                steps {
                    echo 'checking out git repo'                    
                }
            }
            stage('Build') {
                steps{
                    echo 'building.....'
                }
            }
            stage('Test') {
                steps{
                    echo 'testing....'
                }
                
            }
            stage('Deploy'){
                steps{
                    sh 'echo \'hello\''
                }   
                
            }
        }

    post{
        always {
            echo 'post stage initiated'
        
        }
        success {
            echo 'good job it works'
        }
        failure {
            echo 'you made a mistake, something doesnt work'
        }
    }
}
