pipeline {
    agent any

    stages {

        stage('Deploy') {
            steps {
                echo "Deploying to Apache..."

                sh '''
                rm -rf /var/www/html/*
                cp -r * /var/www/html/
                '''
            }
        }

    }
}
