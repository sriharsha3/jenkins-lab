pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }

        stage('Workspace Info') {
            steps {
                sh 'pwd'
                sh 'ls -lrth'
            }
        }
    }
}
