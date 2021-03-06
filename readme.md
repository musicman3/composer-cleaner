Victor The Cleaner for Composer
===============================

[![Downloads this Month](https://img.shields.io/packagist/dm/dg/composer-cleaner.svg)](https://packagist.org/packages/dg/composer-cleaner)
[![Build Status](https://travis-ci.org/dg/composer-cleaner.svg?branch=master)](https://travis-ci.org/dg/composer-cleaner)

This tool removes unnecessary files and directories from Composer vendor directory.

Installation
------------

```
composer require dg/composer-cleaner
```

Then simply use `composer update`.


Configuration
-------------

You can also specify paths to be ignored (ie they will not be deleted) via `composer.json`:

```js
{
	"extra": {
		"cleaner-ignore": {
			"slevomat/eet-client": [  // name of package
				"wsdl*"               // files or subdirectories, you can use wildcards `*` and `?`
			],

			"mpdf/mpdf": true         // ignores whole package
		}
	}
}
```

If you like it, **[please make a donation now](https://nette.org/make-donation?to=composer-cleaner)**. Thank you!
