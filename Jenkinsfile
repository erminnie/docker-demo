pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 5000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
