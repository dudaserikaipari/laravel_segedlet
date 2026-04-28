# laravel_segedlet
composer create-project laravel/laravel [projektneve]

Majd a létrejött projekt könyvtárba lépve:
php artisan install:api

database/migrations => törlés

.env beállítások => XAMPP/PhpMyadmin beállítástól is függ (pl. portszám, user, password)
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=adatbazisneve
DB_USERNAME=root
DB_PASSWORD=

php artisan make:model -c --api [Név] (migráció esetén -mc)
php artisan serve

routes/api.php => útvonalak felvétele api nélkül!!!
minden kérés urlben: http://localhost:8000/api/valami

TIPP: ha a session miatti hiba zavar, akkor a config/session.php állományban:
'driver' => ‘null’,
