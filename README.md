 
### 1. Copy the `.env.example` file

We need to specify our Environment variables for our application. You will see a file named `.env.example`, you will need to duplicate that file and rename it to `.env`.

Then, open up the `.env` file and update your *DB_DATABASE*, *DB_USERNAME*, and *DB_PASSWORD* in the appropriate fields. You will also want to update the *APP_URL* to the URL of your application.

 
### 2. Add Composer Dependencies

First, you should ensure that your web server has the required PHP extensions installed:

> [Laravel PHP Requirements](https://laravel.com/docs/9.x/deployment#server-requirements)

Following that, we'll need to install all composer dependencies through the following command:
```php
composer install
```

### 34. Run Migrations and Seeds

We must migrate our database schema into our database, which we can accomplish by running the following command:
```php
php artisan migrate
```
<br>
Finally, we will need to seed our database with the following command:

```php
php artisan db:seed
```
<br>
 