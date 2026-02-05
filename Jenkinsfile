pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo "Cloning code..."
                git 'https://github.com/Sethuamuthan/pharmacy-app.git'
            }
        }

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
