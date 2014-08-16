#Paginator (PHPExtra\Paginator)

[![Latest Stable Version](https://poser.pugx.org/phpextra/paginator/v/stable.svg)](https://packagist.org/packages/phpextra/paginator)
[![Total Downloads](https://poser.pugx.org/phpextra/paginator/downloads.svg)](https://packagist.org/packages/phpextra/paginator)
[![License](https://poser.pugx.org/phpextra/paginator/license.svg)](https://packagist.org/packages/phpextra/paginator)
[![Build Status](http://img.shields.io/travis/phpextra/paginator.svg)](https://travis-ci.org/phpextra/paginator)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/phpextra/paginator/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/phpextra/paginator/?branch=master)
[![Code Coverage](https://scrutinizer-ci.com/g/phpextra/paginator/badges/coverage.png?b=master)](https://scrutinizer-ci.com/g/phpextra/paginator/?branch=master)
[![GitTip](http://img.shields.io/gittip/jkobus.svg)](https://www.gittip.com/jkobus)

##Usage

Paginator is fully compatible with Collection (PHPExtra/Collection). It's task is to split large collections into pages.

```php
$page = 2;
$itemsPerPage = 10;
$products = new Collection(...);
$paginator = new Paginator($products, $page, $itemsPerPage);

echo $paginator->getPage(); // returns a collection with size of 10 for current page
echo $paginator->getNextPageNumber(); // returns "3"
echo $paginator->hasNextPage(); // returns bool true or false
```

##Changelog

    No release yet

##Contributing

All code contributions must go through a pull request.
Fork the project, create a feature branch, and send me a pull request.
To ensure a consistent code base, you should make sure the code follows
the [coding standards](http://symfony.com/doc/2.0/contributing/code/standards.html).
If you would like to help take a look at the **list of issues**.

##Requirements

    See **composer.json** for a full list of dependencies.

##Authors

    Jacek Kobus - <kobus.jacek@gmail.com>

## License information

    See the file LICENSE.txt for copying permission.