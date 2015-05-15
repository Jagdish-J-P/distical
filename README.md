# Distical

[![Build Status](https://scrutinizer-ci.com/g/bobsta63/distical/badges/build.png?b=master)](https://scrutinizer-ci.com/g/bobsta63/distical/build-status/master)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/bobsta63/distical/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/bobsta63/distical/?branch=master)
[![Latest Stable Version](https://poser.pugx.org/ballen/distical/v/stable)](https://packagist.org/packages/ballen/distical)
[![Latest Unstable Version](https://poser.pugx.org/ballen/distical/v/unstable)](https://packagist.org/packages/ballen/distical)
[![License](https://poser.pugx.org/ballen/distical/license)](https://packagist.org/packages/ballen/distical)

Distical is a PHP distance calculator library of which, amongst other things is developed to calculate the distance between two or more lat/long coordinates.

## License

This client library is released under the [MIT license](LICENSE).

## Requirements

This library is developed and tested for PHP 5.3+

This library is unit tested against PHP 5.3, 5.4, 5.5, 5.6, HHVM and 7.0!

## Setup

I highly recommend the use of [Composer](https://getcomposer.org/) when installing and using this library, it is not mandatory however and you can use a provided 'include' script to load in this library if required.

### Composer

To add this library to your project, edit your ``composer.json`` file and add the following lines (or update your existing ``require`` section with the library like so):

```php
"require": {
        "ballen/distical": "~2.0"
}
```

Then install the package like so:

```
composer install ballen/distical --no-dev
```

### Standalone

You can use the library "standalone" by downloading it from the [GitHub releases section](https://github.com/bobsta63/distical/releases), extracting the files to a place on your server and then adding the "include" into your code like so:

```php
require_once 'path/to/Distical/Distical.inc.php';
```

## Examples

A set of working examples can be found in the ``/examples`` directory.

## Tests and coverage

This library is fully unit tested using [PHPUnit](https://phpunit.de/).

I use TravisCI for continuous integration, which triggers tests for PHP 5.3, 5.4, 5.5, 5.6, 7.0 and HHVM everytime a commit is pushed.

If you wish to run the tests yourself you should run the following:

```
# Install the Distical Library with the 'development' packages this then including PHPUnit!
composer install --dev
# Now we run the unit tests (from the root of the project) like so:
./vendor/bin/phpunit
```

Code coverage can also be ran but rquires XDebug installed...
```
./vendor/bin/phpunit --coverage-html ./report
```

## Support

I am happy to provide support via. my personal email address, so if you need a hand drop me an email at: [ballen@bobbyallen.me](mailto:ballen@bobbyallen.me).