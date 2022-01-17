## About

Docker-compose repository with \
php 8 (Dockerfile: /php-fpm), \
nodeJS 14.18.2 (Dockerfile: /nodejs), \
mariaDB (after build stores in /databases), \
NGINX and Certbot (for https certificates). \
Configs stored in /conf.

## Setup

1. First you must setup certificates like it is described in this post - https://pentacent.medium.com/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71 . init-letsencrypt.sh in this repo already setup for api.bestmester-massage.ru
2. install Laravel api application in /api directory (no subdirectories) and NuxtJS app in /nuxt
3. Run commands below
```
    //build
    $ sudo docker-compose build
    
    //run
    $ sudo docker-compose up -d
```