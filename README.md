# laravel-svelte
En este repositorio se describirán los pasos para usar Svelte, dentro de Laravel, como suele pasar con Vue.

`laravel new laravel-svelte`

`cd laravel-svelte`

`composer require wewowweb/laravel-svelte-preset`

`php artisan preset svelte`

`npm install && npm run dev`

reemplazar el contenido de wellcome.blade.php por

`<!doctype html>`

`<html lang="{{ str_replace('_', '-', app()->getLocale()) }}">`

`<head>`

`<meta charset="utf-8">`

`        <meta name="viewport" content="width=device-width, initial-scale=1">`

`        <title>Laravel</title>`

`        <!-- Fonts -->`

`          <link href="https://fonts.googleapis.com/css?family=Nunito:200,600" rel="stylesheet">`

`          <link rel="stylesheet" href="{{ asset('css/app.css') }}">`

`          </head>`

`       <body>`

`           <script src="{{ asset('js/app.js') }}"></script>`

`       </body>`

`</html>`
