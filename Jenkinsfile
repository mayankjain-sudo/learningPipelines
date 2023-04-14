pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                checkout scm
                sh "ls -altr" 
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh "cat hello.sh"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh "./hello.sh"
            }
        }
    }
}