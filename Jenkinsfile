pipeline {
    agent any

    stages {
        stage('Install dependencies') {
            steps {
                sh 'npm ci'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
