# laravel-docker

Create a local Laravel dev environment with Docker

### Setup

#### Install composer

```
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
chmod +x /usr/local/bin/composer

composer

```

sudo apt-get update
sudo apt install php-xml
sudo apt-get install php-mbstring
sudo chmod -R 777 ./

#### Setup laravel project:

composer create-project laravel/laravel .
php artisan key:generate

#### Change db config

```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=laravel
DB_PASSWORD=password
```

Run
docker-compose exec php php /var/www/html/artisan migrate
