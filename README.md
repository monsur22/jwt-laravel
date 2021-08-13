<h1>Ref: <a href="https://programmingfields.com/create-rest-api-in-laravel-8-using-jwt-authentication/?ref=morioh.com">JWT Laravel</a></h1>
<p>composer create-project --prefer-dist laravel/laravel jwt-auth-api</p>
<p>CREATE DATABASE laravel_jwt;</p>
<p>composer require tymon/jwt-auth
</p>
<p>
In order to add provider and alias for the JWT package, navigate to the config/app.php file.

config/app.php
    'providers' => [

        ...
        ...
        ...
        Tymon\JWTAuth\Providers\LaravelServiceProvider::class,
    ],


    'aliases' => [
        ...
        ...
        ...
        'JWTAuth' => Tymon\JWTAuth\Facades\JWTAuth::class,
        'JWTFactory' => Tymon\JWTAuth\Facades\JWTFactory::class,
    ],
</p>
<p>php artisan jwt:secret</p>
<p>use namespace for jwt auth
use Tymon\JWTAuth\Contracts\JWTSubject;</p>
<p></p>
<p></p>
<p></p>
<p></p>
