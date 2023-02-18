pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'
                sh error
                echo 'Build Completed'
            }
        }
        stage('Test') {
            steps {
                echo 'Starting Testing'
                sh './PES2UG20CS025.exe'
                echo 'Test Completed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Starting Deploy'
                echo 'Deploy Completed'
            }
        }
    }
  post {
    failure {
      echo 'Pipeline Failed'
    }
  }
}
