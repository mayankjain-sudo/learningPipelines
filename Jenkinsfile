pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                checkout scm
                echo "Hello World!"
                sh "ls"
                sh "hostname"
                sh "uptime"
            }
        }
    }
}