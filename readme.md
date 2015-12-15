## Laravel Sky Blank

Laravel Customized Version

Currently at Laravel Framework version 5.1.26 (LTS)


** composer self-update

** composer require laravelcollective/html

** composer require caffeinated/modules

** composer require intervention/image

** composer require roumen/feed

** composer require maatwebsite/excel

artisan vendor:publish --provider="Intervention\Image\ImageServiceProviderLaravel5"


artisan vendor:publish


## Configuration

'timezone' => 'Asia/Manila',

config

Service Provider

Caffeinated\Modules\ModulesServiceProvider::class,
Collective\Html\HtmlServiceProvider::class,
Intervention\Image\ImageServiceProvider::class,
Roumen\Feed\FeedServiceProvider::class,
Maatwebsite\Excel\ExcelServiceProvider::class,


Facade

'Module' => Caffeinated\Modules\Facades\Module::class,
'Form' => Collective\Html\FormFacade::class,
'Html' => Collective\Html\HtmlFacade::class,
'Image' => Intervention\Image\Facades\Image::class

## Usage

#### Intervention

Route::get('/', function()
{

    $img = Image::make('foo.jpg')->resize(300, 200);

    return $img->response('jpg');

});



## Why this version

This customized version was created to facilitate our development in Laravel and pre-packaged to allow agile development.



## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](http://laravel.com/docs/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell at taylor@laravel.com. All security vulnerabilities will be promptly addressed.

### License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)
