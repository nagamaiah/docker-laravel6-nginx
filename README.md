# docker-laravel6-nginx
Laravel6 project with docker setup php7.4-fpm , nginx and mysql
## clone repo and cd docker/ dir
Run docker-compose up -d --build
## add entry in /etc/hosts file
127.0.0.1 laravel6-docker.com
## brose site with following url
http://laravel6-docker.com:8880/
## you connect to phpmyadmin using
http://localhost:8081 \
username : laravel6 \
password : secret
