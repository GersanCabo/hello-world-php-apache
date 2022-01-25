pipeline {
    agent { docker { image 'php:7.4-cli' } }
    stages {
        stage('build') {
            steps {
                git clone https://github.com/GersanCabo/hello-world-php-apache
                sudo docker build -t hello-world-php-apache .
                sudo docker run -p 80:80 hello-world-php-apache
            }
        }
    }
}