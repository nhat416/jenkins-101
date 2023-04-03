pipeline {
    agent {
        node {
            label 'docker-agent-python'
        }
    }
    triggers {
        pollSCM '*/1 * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh '''
                echo "Build item..."
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing..."
                sh '''
                echo "Test item..."
                '''
            }
        }
        stage("Deploy") {
            steps {
                echo 'Deploying...'
                sh '''
                echo "Deploying item..."
                '''
            }
        }
    }
}
