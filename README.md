
# Laravel (PHP 7.4) Docker Setup

Hi! Geeks This is Laravel default setup using PHP 7.4 version using docker.

## How to Run


```bash

  git clone https://github.com/Gurinder-Batth/laravel-7.4-docker-setup.git
  
  cd laravel-7.4-docker-setup

  docker-compose up -d
  # Make sure you have latest version of docker compose https://github.com/docker/compose/releases
  # In this project I used  v2.6.1 of docker compose
  # This above things take time start the docker containers

 docker exec <laravel_container_id> composer install
  
```


## After run open followig url in browser


```bash
  http://127.0.0.1:1234

  #Note: No need to run php artisan serve because laravel serve by apache.
```

## How to Run composer, php, artisan and mysql


```bash
  docker exec <laravel_container_id> composer -v

  docker exec <laravel_container_id> php artisan migrate

  docker exec -it <mysql_container_id> mysql -u user -p
  # password is password 

  # Get all the container id following command and look for laravel laravelserver and laraveldb

  docker ps 
  
```

## Where Laravel Setup


```bash
  /src
```


## Where Apache Config


```bash
  /apache
```
## Features

- No extra stuff included you can install on per your requirement


## Authors

- [@Gurinder-Batth](https://github.com/Gurinder-Batth/)


## License

[MIT](https://choosealicense.com/licenses/mit/)


