# Drupal 8 w/Docker
This repo contains a Drupal installation setup to use Docker to create a development environment. This repo can be used as a starting point for developing Drupal 8 apps with Docker.

This setup contains;

 - PHP-FPM (PHP 7)
 - Nginx web server
 - MySQL database

## Run
Make sure your have composer and [Docker](https://docs.docker.com/) installed

  Create project folder

    mkdir project_name

  Change directory

    cd project_name

  Clone the repo

    git clone git@github.com:saidatom/compose-d8.git .

  Add Laravel to folder

    git clone [project] .

  Install dependencies

    composer install
  Build and run the Docker containers

    docker-compose up -d

  This builds the containers and runs them in the background, while this
     docker-compose up
   builds the containers to outputs their logs to the console.
   Add to hosts [127.0.0.1 local.localhost.me]
   You should be able to visit your app at http://local.localhost.me

To stop the containers run `docker-compose kill`, and to remove them run `docker-compose rm`
