pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:23'
                    reuseNode true
                }
            }
            steps {
                sh '''
                    ls -la
                    node --version
                    npm --version
                    ls -la
                '''
            }
        }
    }
}
