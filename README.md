# Sub Platform

## Installation Setup
1. Clone the repository
2. Run `composer install` to install the dependencies.
3. Run `cp .env.example .env` to generate your local `.env` file.
4. Run `php artisan key:generate` to generate your application key.
5. Open your `.env` and configure your database credentials.
6. Run `php artisan migrate --seed`
7. Finally `php artisan serve`

## Documentation
https://documenter.getpostman.com/view/9517386/UVyyttEc

## Queue
The post notification to subscribers are queued, so you will need to run `php artisan queue:listen`

## Command
There is a command to send "post-created" emails to subscribers: `php artisan send:notification`.

