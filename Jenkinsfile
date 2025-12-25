pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                echo 'Code download ho raha hai...'
                git branch: 'master',
                    url: 'https://github.com/Aimen12782/web2'
            }
        }

       stage('Deploy Website') {
            steps {
                bat '''
                mkdir C:\\deploy 2>nul
                xcopy * C:\\deploy\\ /E /Y /I
                '''
            }
        }
    }
}
