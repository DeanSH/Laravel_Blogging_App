# LSAPP - Laravel From Scratch App

This is the source code for the "Laravel From Scratch" Youtube series by Traversy media. It is a website with a blog application. It also includes full authentication and file uploading. I followed the tutorial then modified it to start becoming an Auction market place mockup (uncompleted).

## Version
1.0.0

## Database
The sql dump is in _SQL/lsapp.sql

## Laravel Command Notes:

cd ~\Desktop\practice_app

-> Create project/install Laravel using composer:
composer create-project --prefer-dist laravel/laravel practice_app

-> Change directory:
cd practice_app

-> Host Web Server for Laravel:
php artisan serve

-> Navigate to the hosted server:
http://localhost:8000

-> Delete vendor folder and composer.lock files when pushing live or sharing it.

-> Run this again in project directory to put the composer.lock files back or to run someone elses project..
composer install

-> enter maintenace mode (run in other cmd):
php artisan down

-> then to go back live:
php artisan up

-> clear our website cache:
php artisan cache:clear

-> to make a controller (app/http/controllers):
php artisan make:controller ClientController

-> to make a model (app/)
php artisan make:model Client

-> to create a model with migration?? wtf (app/)
-> I think it means it also creates a database structure file to match the specified class.
php artisan make:model Room -m

-> Make a class/ model read only
php artisan make:model ReadOnlyBase

-> MYSQL Command to create account to access local DB instead of root.	
CREATE USER 'Dea'@'localhost' IDENTIFIED BY 'Dea';

-> Grant the acc permissions to the schema all previledges
GRANT ALL PRIVILEGES ON deadb.* TO 'Dea'@'localhost';

-> Database Files in Laravel to update SQL connection
/config/database.php and .env file do next command clear cache!

-> Clear the cache files for the local server hosting.
php artisan config:clear
