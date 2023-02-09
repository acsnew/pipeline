pipeline {
    agent any

    stages {
        stage('Change Permissions') {
            steps {
                sh 'sudo chmod +x build.sh'
            }
        }

        stage('Build') {
            steps {
                sh 'sudo ./build.sh'
            }
        }

        stage('Test') {
            steps {
                sh 'sudo ./test.sh'
            }
        }
    }
}

