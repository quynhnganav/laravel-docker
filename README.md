- Required: Docker
- docker build -t localcomposer -f ./composer/composer.Dockerfile ./composer
- docker run -v ${pwd}/app:/var/www/html localcomposer:latest composer install
- docker-compose up -d
- docker-compose exec app php artisan key:generate# laravel-docker
# laravel-docker
