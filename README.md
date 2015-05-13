# lc-genconf

A Wordpress plugin that eases the creation of configuration pages for other plugins.

## Features

- A configuration page is described in a PHP array, pass that to lc-wpgenconf with an identifier and it takes care of the rest
- A configuration can be repeated ("add" and "remove" buttons)
- A set of fields can be displayed conditionnaly, based on the value of another field

## Install

Just as any other WordPress plugin, copy the `lc-genconf` folder in `wp-content/plugins/` then activate it in the Wordpress configuration

## Usage

- Define a function named `yourid_configuration_defintion()` returning the array describing the configuration (see [documentation](https://github.com/louiscarrese/lc-wpgenconf/wiki/configuration_array#configuration-array))
- Call `lc_genconf('yourid')` to get the HTML fragment.

## Known limitations

### Disclaimer
This plugin has been developped aside other plugins of mine. It does what I need for those plugins and not much more.

### Supported fields
As of today, only those types of fields can be defined (more can be added as I need them or if asked) :
- Text
- Checkbox
- Dropdown list
- Category list (wp_dropdown_categories)

