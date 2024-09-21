pipeline {
    agent any

    stages {
        stage('checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/boateng0303/staticapp.git'
            }
        }
        stage('build'){
            steps{
                sh 'echo build'
            }
        }

        stage('test'){
            steps{
                sh 'echo test'
            }
        }

    }
}