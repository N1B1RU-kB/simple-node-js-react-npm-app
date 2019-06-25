pipeline {
    agent 
    {
        docker 
        {
            image 'node:6-alpine' 
            args '-p 3004:3004' 
        }
    }
    stages 
    {
        stage('Build') 
        { 
            steps 
            {
                sh 'npm install' 
            }
        }
        stage('Test') 
        { 
            steps 
            {
                sh 'npm ./jenkins/scripts/test' 
            }
        }
    }
}
