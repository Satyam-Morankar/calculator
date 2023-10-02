pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                checkout scm
                executeShell 'npm install'
                executeShell 'npm run test -- --watchAll=false'
                executeShell 'npm run build'
            }
        }
    }
}
