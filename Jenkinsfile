pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                checkout scm
                echo "Hello World!"
                sh "echo Hello from the shell"
                sh "hostname"
                sh "uptime"
            }
        }
    }
}