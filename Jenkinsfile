pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3004:3004' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        stage('Build') { 
            steps {
                sh 'simple-node-js-react-npm-app/jenkins/scripts/test.sh' 
            }
        }
    }
    }
}
