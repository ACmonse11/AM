pipeline {
    agent {
        docker {
            image 'node:18'
            args '-u root:root -v /var/run/docker.sock:/var/run/docker.sock'
        }
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/ACmonse11/AM.git'
            }
        }

        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Package Docker image') {
            steps {
                sh '''
                docker build -t am-landing:latest .
                '''
            }
        }
    }

    post {
        failure {
            echo '❌ Build failed.'
        }
        success {
            echo '🎉 Build success!'
        }
    }
}
