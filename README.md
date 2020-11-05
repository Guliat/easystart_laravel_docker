## About Repository
  - Laravel 8.13.0
  - Jetstream 1.6.0
  - Livewire 2.3.1

## Docker
  - I use <a href="https://github.com/aschmelyun/docker-compose-laravel" target="_blank">THIS</a> repo by Andrew Schmelyun.
  - ADDRESS: localhost
  - PORT: 85

## Installation
  - Clone repo
  - enter into repo folder
  - docker-compose up -d --build site
  - Copy and config .env file
  - docker-compose run --rm composer install
  - docker-compose run --rm artisan key:generate
  - docker-compose run --rm artisan migrate
  <b>- !! storage symlink ??</b>
