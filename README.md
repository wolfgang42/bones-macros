[![Build Status](https://travis-ci.org/GeneaLabs/bones-macros.svg?branch=master)](https://travis-ci.org/GeneaLabs/bones-macros) [![Latest Stable Version](https://poser.pugx.org/genealabs/bones-macros/v/stable.svg)](https://packagist.org/packages/genealabs/bones-macros) [![Latest Unstable Version](https://poser.pugx.org/genealabs/bones-macros/v/unstable.svg)](https://packagist.org/packages/genealabs/bones-macros) [![License](https://poser.pugx.org/genealabs/bones-macros/license.svg)](https://packagist.org/packages/genealabs/bones-macros)

# Laravel Bones Macros (bones-macros) 

## Installation

To install bones-flash as a stand-alone module:

```sh
composer require "genealabs/bones-macros":"*"
```

or add it to you composer.json file:

```json
    "require": {
        /* ... */,
        "genealabs/bones-macros": "*"
    },
    /* ... */
```

And then add the service provider to your app.php config file:
```php
	// 'providers' => array(
		'GeneaLabs\BonesMacros\BonesMacrosServiceProvider',
    // );
```

## Usage

These HTML and FORM macros are intended to be used mainly in Blade tempaltes to reduce tedium.

## Methods

The following methods are available to use:

```php
// provides a Bootstrap-compatible cancel button that will take you to the previous page.
{{ Form::cancelButton() }}

// provides a select list with a range of intervals
{{ Form::selectRangeWithInterval($name, $start, $end, $interval, $default = null, $attributes = []) }}

// provides ability to slugify any text
{{ HTML::slugify($text) }}
```

## Dependencies

At this time this package requires:

- Laravel 4.2+
- Bootstrap 3.1+
