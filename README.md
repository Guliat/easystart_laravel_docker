<h1> DO NOT USE THIS REPO YET</h1>

## TODO
  - mysql folder
  - symlink
  - storage folder (profile pictures, etc)
  - test on linux, mac, windows
  - mysql folder permissions
  
## About Repository
  - Laravel 8.13.0
  - Jetstream 1.6.0 (without Teams)
    - To enable Teams uncomment "Features::teams()" in config/jetstream.php
  - Livewire 2.3.1
  - Docker environment - ONLY for development

## Docker
  - I use <a href="https://github.com/aschmelyun/docker-compose-laravel">THIS</a> repo by Andrew Schmelyun.
  - Address: localhost
  - Port: 80
    - If not use 80, stored users files can't be accessed (ex. profile picutre).

## Usage
  - One time only
    - Clone this repo
    - Enter into repo folder
    - Remove .git folder
    - Enter into "src" folder, duplicate .env.example file and rename it to .env
      - No changes nedded !
    - docker-compose up -d --build site
    - docker-compose run --rm composer install
    - docker-compose run --rm artisan key:generate
    - docker-compose run --rm artisan migrate
    - docker-compose run --rm artisan storage:link

 - Every day usage
    - START - docker-compose up -d --build site
    - STOP - docker-compose down

## Notes
  - The Laravel project is in "src" folder
  - If you use Git, initialize new repository into "src" folder
  - If fresh database is needed you can delete "mysql" folder
    - First stop the containers and start them again after deletion
