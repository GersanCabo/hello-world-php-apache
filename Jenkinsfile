pipeline {
    agent { docker { 'php:7.4-cli' } }
    stages {
        stage('build') {
            steps {
                sh 'sudo docker build -t hello-world-php-apache .'
                sh 'sudo docker run -d --rm -p 8084:80 hello-world-php-apache'
            }
        }
    }
}