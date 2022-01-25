pipeline {
    agent { docker { image 'php:7.4-cli' } }
    stages {
        stage('build') {
            steps {
                sudo docker build -t hello-world-php-apache .
                sudo docker run -p 8084:80 hello-world-php-apache
            }
        }
    }
}