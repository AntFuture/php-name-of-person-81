# Name of Person

[![Latest Version on Packagist](https://img.shields.io/packagist/v/imliam/php-name-of-person.svg)](https://packagist.org/packages/imliam/php-name-of-person)
[![Build Status](https://img.shields.io/travis/imliam/php-name-of-person.svg)](https://travis-ci.org/imliam/php-name-of-person)
![Code Quality](https://img.shields.io/scrutinizer/g/imliam/php-name-of-person.svg)
![Code Coverage](https://img.shields.io/scrutinizer/coverage/g/imliam/php-name-of-person.svg)
[![Total Downloads](https://img.shields.io/packagist/dt/imliam/php-name-of-person.svg)](https://packagist.org/packages/imliam/php-name-of-person)
[![License](https://img.shields.io/github/license/imliam/php-name-of-person.svg)](LICENSE.md)

Present names for English-language applications where a first and last name combined is sufficient. This approach does not cover all possible naming cases, deal with other languages or titles.

This is a rough port of [the Ruby package of the same name from Basecamp](https://github.com/basecamp/name_of_person).

<!-- TOC -->

- [Name of Person](#name-of-person)
    - [💾 Installation](#💾-installation)
    - [📝 Usage](#📝-usage)
    - [✅ Testing](#✅-testing)
    - [🔖 Changelog](#🔖-changelog)
    - [⬆️ Upgrading](#⬆️-upgrading)
    - [🎉 Contributing](#🎉-contributing)
        - [🔒 Security](#🔒-security)
    - [👷 Credits](#👷-credits)
    - [♻️ License](#♻️-license)

<!-- /TOC -->

## 💾 Installation

You can install the package with [Composer](https://getcomposer.org/) using the following command:

```bash
composer require imliam/php-name-of-person:^1.0.0
```

## 📝 Usage

``` php
$name = new \ImLiam\NameOfPerson\Name('David Heinemeier Hansson');

$name->getFirstName();      // "David"
$name->getLastName();       // "Heinemeier Hansson"
$name->getInitials();       // "DHH"
$name->getInitials(true);   // "D.H.H."
$name->getFamiliar();       // "David H."
$name->getAbbreviated();    // "D. Heinemeier Hansson"
$name->getSorted();         // "Heinemeier Hansson, David"
$name->getMentionable();    // "davidh"
$name->getPossessive();     // "David Heinemeier Hansson's"
```

## ✅ Testing

``` bash
composer test
```

## 🔖 Changelog

Please see [the changelog file](CHANGELOG.md) for more information on what has changed recently.

## ⬆️ Upgrading

Please see the [upgrading file](UPGRADING.md) for details on upgrading from previous versions.

## 🎉 Contributing

Please see the [contributing file](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md) for details on contributing to the project.

### 🔒 Security

If you discover any security related issues, please email liam@liamhammett.com instead of using the issue tracker.

## 👷 Credits

- [Liam Hammett](https://github.com/imliam)
- [Basecamp](https://github.com/basecamp/name_of_person) for the original Ruby gem
- [All Contributors](../../contributors)

## ♻️ License

The MIT License (MIT). Please see the [license file](LICENSE.md) for more information.
