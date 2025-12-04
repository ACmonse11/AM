pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/ACmonse11/AM.git'
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

        stage('Push to GitHub') {
            steps {
                sh '''
                    git config user.email "jenkins@local"
                    git config user.name "Jenkins"

                    git add .
                    git commit -m "CI: Jenkins auto build" || echo "No changes"
                    git push origin master
                '''
            }
        }
    }

    post {
        success {
            echo 'Build OK — Vercel will deploy automatically.'
        }
        failure {
            echo 'Build failed.'
        }
    }
}
