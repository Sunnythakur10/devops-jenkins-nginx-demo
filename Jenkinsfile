pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/YOUR_USERNAME/devops-jenkins-nginx-demo.git'
            }
        }

        stage('Deploy to Nginx') {
            steps {
                bat '''
                xcopy /E /I /Y *.html C:\\nginx\\html
                xcopy /E /I /Y *.css  C:\\nginx\\html
                '''
            }
        }
    }
}
