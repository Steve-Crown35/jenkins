pipeline {
    agent { 
        node {
            label 'docker-agent-python'
            }
    }        
    triggers {
      pollSCM '* * * * *'
      }
    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh '''
                echo "Building the application now..."
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing..."
                sh '''
                echo "Testing the application now..."
                '''
            }
        }
        stage('Deployment') {
            steps {
                echo 'Deploying...'
                sh '''
                echo "Deploying the application now..."
                '''
            }
        }
    }
}
