## Overview

This extension improves default features of Magento API.

It allows you to:

* Associate simple products to configurable or grouped product;
* Specify category names rather than the ids;
* Specify the name of the attribute set rather than the id;
* Specify options labels rather than the ids;
* Specify the website code rather than the id.

## Installation

### [Composer](http://getcomposer.org)

> A prerequisite for using this method is that you have Composer [installed](http://getcomposer.org/doc/00-intro.md#installation-nix) in your system.

Begin by creating a `composer.json` in the root of Magento, and ensure it has the following:

```json
{
    "repositories": [
        {
           "type": "vcs",
           "url": "https://github.com/magento-hackathon/magento-composer-installer"
        }
    ],
    "require": {
        "magento-hackathon/magento-composer-installer": "*",
        "aoepeople/magento-improve-api": "dev-master"
    },
    "extra": {
        "magento-root-dir": "./",
        "magento-deploystrategy": "copy"
    },
    "config": {
        "preferred-install": "dist"
    }
}
```

Finish by installing Composer dependencies and a couple of optional enhancements:

```bash
cd your-project/
composer install
```

### [modman](https://github.com/colinmollenhour/modman)

    $ modman clone https://github.com/AOEpeople/magento-improve-api.git
    
### Oder installation alternatives
    
#### [modgit](https://github.com/jreinke/modgit):

    $ cd /path/to/magento
    $ modgit init
    $ modgit clone magento-improve-api https://github.com/AOEpeople/magento-improve-api.git

##### download package manually

* Download latest version [here](https://github.com/AOEpeople/magento-improve-api/archive/master.zip)
* Unzip in Magento root folder
* Clear cache    

## How to associate simple products to configurable/grouped product

Please refer to [this article](http://www.bubblecode.net/en/2012/04/20/magento-api-associate-simple-products-to-configurable-or-grouped-product/).
