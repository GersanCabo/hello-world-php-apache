pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'sudo docker build -t hello-world-php-apache .'
                sh 'sudo docker run -d --rm -p 8084:80 hello-world-php-apache'
            }
        }
    }
}