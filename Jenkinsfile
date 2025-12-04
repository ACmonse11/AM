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
                sh '''
                    docker run --rm \
                        -v $PWD:/app \
                        -w /app \
                        node:18 bash -c "
                            npm install &&
                            npm run build
                        "
                '''
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t am-landing:latest .'
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
