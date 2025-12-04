pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/ACmonse11/AM.git'
            }
        }

        stage('Install & Build in Docker Node') {
            steps {
                script {
                    def nodeImage = docker.image('node:18')
                    nodeImage.pull()   // Asegura que existe antes de usarlo

                    nodeImage.inside('-u root:root') {
                        sh 'npm install'
                        sh 'npm run build'
                    }
                }
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t am-landing:latest .'
                }
            }
        }
    }

    post {
        success {
            echo "✔ Build completed successfully."
        }
        failure {
            echo "❌ Build failed."
        }
    }
}
