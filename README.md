# Enum class reflection extension for PHPStan

[![Build Status](https://travis-ci.org/timeweb/phpstan-enum.svg?branch=master)](https://travis-ci.org/timeweb/phpstan-enum)

* [PHPStan](https://github.com/phpstan/phpstan)
* [PHP Enum](https://github.com/myclabs/php-enum)

This extension defines dynamic methods for `MyCLabs\Enum\Enum` subclasses.

## Usage

To use this extension, require it with [Composer](https://getcomposer.org)

```
composer require --dev timeweb/phpstan-enum
```

And include extension.neon in your project's PHPStan config

```
includes:
  - vendor/timeweb/phpstan-enum/extension.neon
```

## Install for Local Development 

### With docker:

```
git clone git@github.com:timeweb/phpstan-enum.git
cd phpstan-enum
make docker-build
make install
make phpunit
```

### Without docker (localy installed actual version of php, composer, etc):

```
git clone git@github.com:timeweb/phpstan-enum.git
cd phpstan-enum
make install
make phpunit
```
