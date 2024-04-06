pipeline {
    agent any
    environment {
        BRANCH_NAME = "${env.BRANCH_NAME}"
    }
    stages {
        stage('build') {
            steps {
                echo "Code checkout"
                checkout scm
            }
        }
        stage('Read variables'){
            steps{
                script{
                    sh 'ls'
                    // Get the value of a variable 
                    def data = readYaml (file: 'vars.yaml')
                    echo "Branch name: ${BRANCH_NAME}"
                    echo "Values: ${data[BRANCH_NAME]}"
                }
            }
        }
    }
}