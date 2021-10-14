pipeline {
    agent any
    stages {
            stage('Git Checkout') {
                steps {
                    echo 'checking out git repo'
                    git credentialsId: '97087b98-3176-47aa-b5b9-21d21e6bcca1', url: 'https://github.com/Kkoonnrraadd/test-repo-for-jenkins.git'
                    echo 'providing letest repo version'
                    
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
