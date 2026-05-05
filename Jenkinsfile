pipeline {
    agent any
    triggers {
        githubPush()
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building the app...'
                sh 'echo build complete'
            }
        }
        stage('Test') {
            steps {
                echo 'Running unit tests...'
                sh 'echo all tests passed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying app...'
                sh 'echo deployed successfully'
            }
        }
    }
    post {
        success {
            echo 'test-pipeline succeeded!'
        }
        failure {
            echo 'test-pipeline failed!'
        }
    }
}
