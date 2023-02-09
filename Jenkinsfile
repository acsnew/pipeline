pipeline {
    agent any

    stages {
        stage('Change Permissions') {
            steps {
                sh 'chmod +x build.sh'
            }
        }

        stage('Build') {
            steps {
                sh './build.sh'
            }
        }

        stage('Test') {
            steps {
                sh './test.sh'
            }
        }
    }
}

