#Laravel 4 - Bootstrap Empowered Application 

This is a Laravel 4 Bootstrap Application. It is a fork off of [andrew13/Laravel-4-Bootstrap](http://github.com/andrew13/Laravel-4-Bootstrap) which includes Twitter Bootstrap 2.2.2 and it comes as an example application to help you get started. This Empowered version adds 3 additional items for improved development speed. 

**`Laravel-4-Bootstrap-Empowered`** contains Laravel 4 composer modules:

- [Confide](#confide)

- [Ardent](#ardent)

- [PowerPack](#powerpack)

##How to install

	git clone git://github.com/andrew13/Laravel-4-Bootstrap-Empowered.git laravel
	cd laravel
	curl -s http://getcomposer.org/installer | php
	php composer.phar install

##Configure
Now that you have the Laravel 4 installed, you need to create a database for it and update the file ***app/config/database.php***



##After that, run these commands to create and populate Users table:

	php artisan migrate:install
	php artisan migrate
	php artisan db:seed


## Make sure app/storage is writable by your web server.
If permissions are set correctly:

    chmod -R 775 app/storage

Should work, if not try

    chmod -R 777 app/storage

##Start Page
Navigate to your Laravel 4 website and try to login with the default credentials:

	email : test@test.com
	password : test

Create a new user at /account/register

<a name="confide"></a>
## Confide Authentication Solution [Confide](https://github.com/Zizaco/confide)

Used for the user auth and registration. In general for user controllers you'll want to use something like the following:

    <?php

    use Zizaco\Confide\ConfideUser;

    class User extends ConfideUser {

    }

For full usage see [Confide Documentation](https://github.com/Zizaco/confide)

<a name="ardent"></a>
## Ardent - Self-validating, secure and smart models for Laravel 4's Eloquent ORM

Used for handling repetitive validation tasks.

For full usage see [Ardent Documentation](https://github.com/laravelbook/ardent) 

<a name="powerpack"></a>
## [Laravel 4 PowerPack](https://github.com/laravelbook/laravel4-powerpack)

Adds string helper classes from Laravel 3 to Laravel 4.

**`laravel4-powerpack`** contains Laravel 4 ports of the following helper classes:

- [HTML](https://github.com/laravelbook/laravel4-powerpack#html_class)

- [Form](https://github.com/laravelbook/laravel4-powerpack#form_class)

- [Str](https://github.com/laravelbook/laravel4-powerpack#str_class)

For full usage see [PowerPack Documentation](https://github.com/laravelbook/laravel4-powerpack)

## License

Confide is free software distributed under the terms of the MIT license

## Aditional information

Any questions, feel free to [contact me](http://twitter.com/andrewelkins).