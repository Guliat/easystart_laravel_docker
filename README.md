## About Repository
  - Laravel 8.13.0
  - Jetstream 1.6.0 - No Teams
    - enable teams in config if needed
  - Livewire 2.3.1
  - Docker environment - ONLY for development

## Docker
  - I use <a href="https://github.com/aschmelyun/docker-compose-laravel">THIS</a> repo by Andrew Schmelyun.
  - Address: localhost
  - Port: 80
    - If not use 80 stored users files can't be accessed (ex. profile picutre).

## Usage
  One time only
    - Clone repo
    - Copy .env.example file and rename it to .env
      - Don't need configuration
    - Enter into repo folder
    - docker-compose up -d --build site
    - docker-compose run --rm composer install
    - docker-compose run --rm artisan key:generate
    - docker-compose run --rm artisan migrate
    - docker-compose run --rm artisan storage:link
  Every day usage
    - docker-compose up -d --build site

## Notes
  - 

## TODO
  - mysql folder
  - symlink
  - storage folder (profile pictures, etc)
  - test on linux, mac, windows
  - mysql folder permissions