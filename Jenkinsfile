pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Deploy to NGINX') {
            steps {
                bat '''
                echo Deploying files to NGINX html folder
                xcopy "%WORKSPACE%\\*" "C:\\Users\\Administrator\\Downloads\\nginx-1.29.4\\nginx-1.29.4\\html\\" /E /I /Y
                '''
            }
        }
    }
}
