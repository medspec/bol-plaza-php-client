[![Build Status](https://travis-ci.org/picqer/bol-plaza-php-client.svg?branch=v2)](https://travis-ci.org/picqer/bol-plaza-php-client)


# Bol.com Plaza API client for PHP
This is an open source PHP client for the [Bol.com Plaza API](https://developers.bol.com/documentatie/plaza-api/).

## Installation
Get it with [composer](https://getcomposer.org)

Run the command:
```
composer require picqer/bol-plaza-php-client
```

## Example: get orders
```php
<?php

require __DIR__ . '/vendor/autoload.php';

$publickey = '--YOUR PUBLIC KEY--';
$privatekey = '--YOUR PRIVATE KEY--';

$client = new Picqer\BolPlazaClient\BolPlazaClient($publickey, $privatekey);

$orders = $client->getOrders();

var_dump($orders);
```

See the [tests file](tests/BolPlazaClientTest.php) for more information.

Thanks to [@mwienk](https://github.com/mwienk) for migrating this package for the Bol Plaza API V2.
