pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                checkout scm
                ls -altr 
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                cat hello.sh
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh hello.sh
            }
        }
    }
}