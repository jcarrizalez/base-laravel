
##JUAN

- creo proyecto:
	composer create-project laravel/laravel team-laravel 7.3.*;
- configuracion de base de datos:
	en mysql: 
		CREATE DATABASE team_laravel;
	en .env:
	DB_DATABASE=team_laravel
	DB_USERNAME=tu_user
	DB_PASSWORD=tu_password
- creo las colas:
	php artisan queue:table;
- refresh:
	composer dumpautoload;
- primer migrate:
	php artisan migrate;

- modifico la vista principal de laravel del get /
	routes/web.php

- creo carpeta packages:
	agrepo extructura de trabajo
	registro package en composer.json
	registro package en config/app.php <- esto por no ser un paquete instalable
		BaseExample\Providers\RegisterProvider::class