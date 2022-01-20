pipeline {
    agent { docker { image 'python:3.10.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                timeout(time: 1, unit: 'MINUTES') {
                    bat 'main.py'
                }

            }
        }
    }
}