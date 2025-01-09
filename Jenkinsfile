pipeline {
    agent {
        docker {
            image 'docker:20.10.24'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'docker pull node:18-alpine'
                sh 'docker inspect -f . node:18-alpine'
            }
        }
    }
}
