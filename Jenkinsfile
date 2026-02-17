pipeline {
    agent {
        docker {
            image 'docker:24.0.5'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }

    stages {

        stage('Check Docker') {
            steps {
                sh 'docker --version'
            }
        }

        stage('Build Script') {
            steps {
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }
    }
}
