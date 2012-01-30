## About

CakePHP make use of special methods in Controller classes known as actions. 
This framework have some own code standards and this important methods could 
be, by example: index, edit and admin_index or admin_view

The last of them break the PEAR standard (NamingConventions.ValidFunctionName 
rule) but as we realy want to use this standard without using CakePHP aliases 
we'll gonna break the standard

## Install

you can find useful tips [here](http://pear.php.net/manual/en/package.php.php-codesniffer.coding-standard-tutorial.php). 
In my case (Ubuntu 10.10) standards are located in 
**/usr/share/php/PHP/CodeSniffer/Standards** *(MacOs information will be welcome)*

By example:

    $ cd /usr/share/php/PHP/CodeSniffer/Standards
        $ git clone git@github.com:moacirosa/phpcs-pear-cakephp.git CakePHPPear

> Keep the target folder (CakePHPPear) with this name to avoid problems like: 
> "Cannot redeclare class..." 
> [check here](http://pear.php.net/bugs/bug.php?id=18751)

## Example

phpcs --standard=CakePHPPear myFile.php

## Issues

Yeap... I'll make these classes agree with this standard
