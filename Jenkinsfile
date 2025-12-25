pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                echo 'Code download ho raha hai...'
                git branch: 'main',
                    url: 'https://github.com/Aimen12782/web2'
            }
        }

        stage('Deploy Website') {
            steps {
                echo 'Website deploy ho rahi hai...'
                bat '''
                rm -rf /var/www/html/*
                cp -r * /var/www/html/
                '''
            }
        }
    }
}
