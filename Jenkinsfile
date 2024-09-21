pipeline {
    agent any


    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/boateng0303/staticapp.git'
    }

    stages {
        stage('checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }
        stage('docker build'){
            steps{
                sh 'docker build -t staticapp .'
                sh 'docker images'
            }
        }

        stage('test'){
            steps{
                sh 'echo test'
            }
        }

    }
}