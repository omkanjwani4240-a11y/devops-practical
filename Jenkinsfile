pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
                echo 'Code downloaded successfully'
            }
        }

        stage('Test Website') {
            steps {
                sh 'test -f index.html'
                echo 'Website test passed!'
            }
        }

        stage('Success') {
            steps {
                echo 'Jenkins pipeline completed!'
            }
        }
    }
}