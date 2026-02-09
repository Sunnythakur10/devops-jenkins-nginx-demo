pipeline {
    agent any

    stages {
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
