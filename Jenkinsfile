pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building or Resolve Dependencies'
                sh 'bundle install'
            }
        }
        stage('Test') {
            steps {
                echo 'Runing Regression Tests'
            }
        }
        stage('UAT') {
            steps {
                echo 'Wait for User Acceptance'
                input(message: 'Go to production?', ok:'Yes')
            }
        }
        stage('Prod') {
            steps {
                echo 'Web App is Ready :D'
            }
        }
    }
}
