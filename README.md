

# String handling evolved

[![Latest Version on Packagist](https://img.shields.io/packagist/v/spatie/string.svg?style=flat-square)](https://packagist.org/packages/spatie/string)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/spatie/string/master.svg?style=flat-square)](https://travis-ci.org/spatie/string)
[![Quality Score](https://img.shields.io/scrutinizer/g/spatie/string.svg?style=flat-square)](https://scrutinizer-ci.com/g/spatie/string)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/860364d5-1d74-4cf8-bdb1-c5e18cdc8a70/mini.png)](https://insight.sensiolabs.com/projects/860364d5-1d74-4cf8-bdb1-c5e18cdc8a70)

This package provides a handy way to work with strings in php.

## Install

You can install this package via composer:

``` bash
composer require spatie/string
```

## Usage

First you must wrap a native string in a String-object. This can be done with the `string`-function.
```
string('myFirstString');
```

From then on you can chain methods like there's no tomorrow

```
echo string('StartMiddleEnd')->between('Start', 'End')->toUpper(); // MIDDLE
``

The following methods are provided:

### between
```php
/**
 * Get the string between the given start and end.
 *
 * @param $start
 * @param $end
 * @return String
 */
public function between($start, $end)
``

Example:
```
string('StartMiddleEnd')->between('Start', 'End')->toUpper(); // MIDDLE
``

### toUpper
```php
/**
 * Convert the string to uppercase.
 *
 * @return String
 */
public function toUpper()
```

Example:
```
string('string')->toUpper(); // STRING
```

### toLower
```php
/**
 * Convert the string to lowercase.
 *
 * @return String
 */
public function toLower()
```

Example:
```
string('STRING')->toLower(); // string
``


## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Testing

You can run the tests with:

```bash
vendor/bin/phpunit
```

## Contributing

We are very happy to receive pull requests to add functions to this class. Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email freek@spatie.be instead of using the issue tracker.

## Credits

- [Freek Van der Herten](https://github.com/freekmurze)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.