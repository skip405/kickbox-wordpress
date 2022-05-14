# Kickbox Verifications using WordPress request functions

[![Packagist](https://img.shields.io/packagist/v/skip405/kickbox-wordpress)](https://packagist.org/packages/skip405/kickbox-wordpress)
[![Packagist](https://img.shields.io/packagist/dt/skip405/kickbox-wordpress)](https://packagist.org/packages/skip405/kickbox-wordpress)

This package provides a Kickbox Email Verification API-client that uses WordPress HTTP-requests functions. Ideal if you want to employ Kickbox email verification in a WordPress plugin or theme.

## Installation
Install via composer:

```
composer require skip405/kickbox-wordpress
```

## Examples

### Verify a single email address
```
// include your composer dependencies
require_once 'vendor/autoload.php';

$client = new Skip405\Kickbox\Client( "KICKBOX_API_KEY" );

$verified_email = $client->verify( "jane.doe@example.com" );
```