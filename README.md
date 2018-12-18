# Paysera PHP library skeleton

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Quality Score][ico-code-quality]][link-code-quality]
[![Total Downloads][ico-downloads]][link-downloads]

This is a skeleton for a new GitHub-based PHP library.

Following steps:
- change `composer.json` file:
  - change `name` and `description` fields;
  - change namespaces;
  - change `type` from `library` to `symfony-bundle` if it's a Symfony bundle;
  - add keywords;
  - add any additional requirements;
- change year (and/or author) in `LICENCE` if needed;
- update this readme:
  - replace all `:vendor/:package_name` occurences with the vendor and name of your library;
  - read and replace TODOs in the readme;
- change / add files in `src` directory, don't forget to modify namespace;
- change / add test cases in `tests` directory, don't forget to modify namespace;
- after pushing initial commit, add the library in [Packagist](https://packagist.org/),
[Travis](https://travis-ci.org/) and [Scrutinizer](https://scrutinizer-ci.com/).

With each relase:
- you can fix code style with `composer fix-cs`;
- you can run tests and code-style checks with `composer test`;
- don't forget to update `CHANGELOG.md`.

To start a library using this skeleton:
```
composer create-project paysera/skeleton-lib directory-name
```

Following readme is just the structure for your new library and is not related
to the skeleton itself.

:red_circle: **TODO: Change this part and title with description about the library.**

## Why?

:red_circle: **TODO: Explain when and why developers should use this library – it's main purpose and/or differences from other solutions.**

You can also rename this to `## Features` or other purpose-like header.

Remove this part if purpose is already clear from the main description.

## Installation

```bash
composer require :vendor/:package_name
```

## Configuration

:red_circle: **TODO: explain bundle configuration or remove this part for non-bundle libraries.**

```yaml
paysera_something:
  field: value
```

## Usage

:red_circle: **TODO: Explain how to use this library. Use code samples for better understanding.**

## Semantic versioning

This library follows [semantic versioning](http://semver.org/spec/v2.0.0.html).

See [Symfony BC rules](http://symfony.com/doc/current/contributing/code/bc.html) for basic
information about what can be changed and what not in the API.

:red_circle: **TODO: Remove following part of this section or use instead of previous one. Remove irrelevant items,
like twig functions, if they are not provided by your library.**

This bundle follows [semantic versioning](http://semver.org/spec/v2.0.0.html).

Public API of this bundle (in other words, you should only use these features if you want to easily update
to new versions):
- only services that are not marked as `public="false"`
- only classes, interfaces and class methods that are marked with `@api`
- twig functions and tags
- console commands
- supported DIC tags

For example, if only class method is marked with `@api`, you should not extend that class, as constructor
could change in any release.

See [Symfony BC rules](https://symfony.com/doc/current/contributing/code/bc.html) for basic information
about what can be changed and what not in the API. Keep in mind, that in this bundle everything is
`@internal` by default.

## Running tests

```
composer update
composer test
```

## Contributing

Feel free to create issues and give pull requests.

You can fix any code style issues using this command:
```
composer fix-cs
```

[ico-version]: https://img.shields.io/packagist/v/:vendor/:package_name.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/:vendor/:package_name/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/:vendor/:package_name.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/:vendor/:package_name.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/:vendor/:package_name.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/:vendor/:package_name
[link-travis]: https://travis-ci.org/:vendor/:package_name
[link-scrutinizer]: https://scrutinizer-ci.com/g/:vendor/:package_name/code-structure
[link-code-quality]: https://scrutinizer-ci.com/g/:vendor/:package_name
[link-downloads]: https://packagist.org/packages/:vendor/:package_name
