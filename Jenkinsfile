pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                checkout scm
                sh 'npm install'
                sh 'npm run test -- --watchAll=false'
                sh 'npm run build'
            }
        }
    }
}