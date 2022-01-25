pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'sudo docker build -t hello-world-php-apache .'
                sh 'sudo docker run -p 8084:80 hello-world-php-apache'
            }
        }
    }
}