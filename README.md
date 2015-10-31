# Laravel-CORS-Middleware

Copy the CORS.php inside app/Http/Middleware/CORS.php

Edit your Kernel.php file

```php
<?php
$middleware = [
       ...
        \App\Http\Middleware\CORS::class
    ];
?>
```
If you need to specify specific alloed domains you can edit

```php
header('Access-Control-Allow-Origin' , '*')
```

> It works with JWT middleware with Authorization header
http://www.codeanchor.net/blog/creating-custom-laravel-5-packages/
