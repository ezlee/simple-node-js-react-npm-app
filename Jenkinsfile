pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000 --privileged' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'id'
                sh 'pwd'
                sh 'ls -al'
                sh 'env|sort'
                sh 'npm config get prefix'
                sh 'npm install' 
            }
        }
    }
}
