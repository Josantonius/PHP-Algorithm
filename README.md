# PHP Algorithm class

[![Latest Stable Version](https://poser.pugx.org/josantonius/Algorithm/v/stable)](https://packagist.org/packages/josantonius/Algorithm) [![Latest Unstable Version](https://poser.pugx.org/josantonius/Algorithm/v/unstable)](https://packagist.org/packages/josantonius/Algorithm) [![License](https://poser.pugx.org/josantonius/Algorithm/license)](LICENSE) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/3505aa3d827b48839fd3f6a2166dbbc6)](https://www.codacy.com/app/Josantonius/PHP-Algorithm?utm_source=github.com&utm_medium=referral&utm_content=Josantonius/PHP-Algorithm&utm_campaign=Badge_Grade) [![Total Downloads](https://poser.pugx.org/josantonius/Algorithm/downloads)](https://packagist.org/packages/josantonius/Algorithm) [![Travis](https://travis-ci.org/Josantonius/PHP-Algorithm.svg)](https://travis-ci.org/Josantonius/PHP-Algorithm) [![PSR2](https://img.shields.io/badge/PSR-2-1abc9c.svg)](http://www.php-fig.org/psr/psr-2/) [![PSR4](https://img.shields.io/badge/PSR-4-9b59b6.svg)](http://www.php-fig.org/psr/psr-4/) [![CodeCov](https://codecov.io/gh/Josantonius/PHP-Algorithm/branch/master/graph/badge.svg)](https://codecov.io/gh/Josantonius/PHP-Algorithm)

[Versión en español](README-ES.md)

Class with algorithms to solve and display mathematical sequences.

---

-   [Requirements](#requirements)
-   [Installation](#installation)
-   [Available Methods](#available-methods)
-   [Quick Start](#quick-start)
-   [Usage](#usage)
-   [Tests](#tests)
-   [TODO](#-todo)
-   [Contribute](#contribute)
-   [Repository](#repository)
-   [License](#license)
-   [Copyright](#copyright)

---

## Requirements

This class is supported by **PHP versions 5.6** or higher and is compatible with **HHVM versions 3.0** or higher...

## Installation

The preferred way to install this extension is through [Composer](http://getcomposer.org/download/).

To install **PHP Algorithm class**, simply:

    $ composer require Josantonius/Algorithm

The previous command will only install the necessary files, if you prefer to **download the entire source code** you can use:

    $ composer require Josantonius/Algorithm --prefer-source

You can also **clone the complete repository** with Git:

    $ git clone https://github.com/Josantonius/PHP-Algorithm.git

Or **install it manually**:

[Download Algorithm.php](https://raw.githubusercontent.com/Josantonius/PHP-Algorithm/master/src/Algorithm.php):

    $ wget https://raw.githubusercontent.com/Josantonius/PHP-Algorithm/master/src/Algorithm.php

## Available Methods

Available methods in this class:

### - Print "Look-and-Say" sequence:

```php
Algorithm::lookAndSay($lastSequence, $maxLines);
```

| Attribute     | Description                         | Type | Required | Default |
| ------------- | ----------------------------------- | ---- | -------- | ------- |
| $lastSequence | Initial value to start the sequence | int  | No       | 1       |
| $maxLines     | Maximum lines number to show        | int  | No       | 15      |

**# Return** (string) → Sequence.

## Quick Start

To use this class with **Composer**:

```php
require __DIR__ . '/vendor/autoload.php';

use Josantonius\Algorithm\Algorithm;
```

Or If you installed it **manually**, use it:

```php
require_once __DIR__ . '/Algorithm.php';

use Josantonius\Algorithm\Algorithm;
```

## Usage

Example of use for this class:

```php
echo Algorithm::lookAndSay();

/*
1
11
21
1211
111221
312211
13112221
1113213211
31131211131221
13211311123113112211
11131221133112132113212221
3113112221232112111312211312113211
1321132132111213122112311311222113111221131221
11131221131211131231121113112221121321132132211331222113112211
311311222113111231131112132112311321322112111312211312111322212311322113212221
*/
```

```php
echo Algorithm::lookAndSay(22, 5);

/*
22
22
22
22
22
*/
```

## Tests

To run [tests](tests) you just need [composer](http://getcomposer.org/download/) and to execute the following:

    $ git clone https://github.com/Josantonius/PHP-Algorithm.git

    $ cd PHP-Algorithm

    $ composer install

Run unit tests with [PHPUnit](https://phpunit.de/):

    $ composer phpunit

Run [PSR2](http://www.php-fig.org/psr/psr-2/) code standard tests with [PHPCS](https://github.com/squizlabs/PHP_CodeSniffer):

    $ composer phpcs

Run [PHP Mess Detector](https://phpmd.org/) tests to detect inconsistencies in code style:

    $ composer phpmd

Run all previous tests:

    $ composer tests

## ☑ TODO

-   [ ] Add new feature.
-   [ ] Improve tests.
-   [ ] Improve documentation.
-   [ ] Refactor code for disabled code style rules. See [phpmd.xml](phpmd.xml) and [.php_cs.dist](.php_cs.dist).

## Contribute

If you would like to help, please take a look at the list of
[issues](https://github.com/Josantonius/PHP-Algorithm/issues) or the [To Do](#-todo) checklist.

**Pull requests**

-   [Fork and clone](https://help.github.com/articles/fork-a-repo).
-   Run the command `composer install` to install the dependencies.
    This will also install the [dev dependencies](https://getcomposer.org/doc/03-cli.md#install).
-   Run the command `composer fix` to excute code standard fixers.
-   Run the [tests](#tests).
-   Create a **branch**, **commit**, **push** and send me a
    [pull request](https://help.github.com/articles/using-pull-requests).

## Repository

The file structure from this repository was created with [PHP-Skeleton](https://github.com/Josantonius/PHP-Skeleton).

## License

This project is licensed under **MIT license**. See the [LICENSE](LICENSE) file for more info.

## Copyright

2017 - 2021 Josantonius, [josantonius.dev](https://josantonius.dev/)

If you find it useful, let me know :wink:

You can contact me on [Twitter](https://twitter.com/Josantonius) or through my [email](mailto:hello@josantonius.dev).


