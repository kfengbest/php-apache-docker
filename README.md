# php-apache-docker

Build the container:

    docker build -t php-apache .

Getting it running

    docker run -p 8080:80 -d php-apache

Shell running

    docker run -i -t -p 8080:80 php-apache /bin/bash
    apachectl start

Mount a directory from host to conainter.

    docker run -p 8080:80 -d -v /Users/kfeng/site:/var/www/site php-apache

