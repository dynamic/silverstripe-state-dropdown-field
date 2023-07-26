# Silverstripe State Dropdown Field

A simple state dropdown field for SilverStripe forms. This dropdown defaults to US states and CA provinces but allows for the source to be overridden.

[![CI](https://github.com/dynamic/silverstripe-state-dropdown-field/actions/workflows/ci.yml/badge.svg)](https://github.com/dynamic/silverstripe-state-dropdown-field/actions/workflows/ci.yml)
[![codecov](https://codecov.io/gh/dynamic/silverstripe-state-dropdown-field/branch/master/graph/badge.svg)](https://codecov.io/gh/dynamic/silverstripe-state-dropdown-field)

[![Latest Stable Version](https://poser.pugx.org/dynamic/state-dropdown-field/v/stable)](https://packagist.org/packages/dynamic/state-dropdown-field)
[![Total Downloads](https://poser.pugx.org/dynamic/state-dropdown-field/downloads)](https://packagist.org/packages/dynamic/state-dropdown-field)
[![Latest Unstable Version](https://poser.pugx.org/dynamic/state-dropdown-field/v/unstable)](https://packagist.org/packages/dynamic/state-dropdown-field)
[![License](https://poser.pugx.org/dynamic/state-dropdown-field/license)](https://packagist.org/packages/dynamic/state-dropdown-field)

## Requirements

* Silverstripe ^4.0

## Installation

`composer require dynamic/state-dropdown-field`

## License

See [License](LICENSE.md)

## Example usage

```php

public function getCMSFields(){
    $fields = parent::getCMSFields();
    
    $fields->addFieldToTab(
        'Root.MyTab',
        \Dynamic\StateDropdownField\Fields\StateDropdownField::create('States', 'States')
    );
    
    return $fields;
}

```

## Maintainers

 *  [Dynamic](https://www.dynamicagency.com) (<dev@dynamicagency.com>)

## Bugtracker
Bugs are tracked in the issues section of this repository. Before submitting an issue please read over
existing issues to ensure yours is unique.

If the issue does look like a new bug:

 - Create a new issue
 - Describe the steps required to reproduce your issue, and the expected outcome. Unit tests, screenshots
 and screencasts can help here.
 - Describe your environment as detailed as possible: SilverStripe version, Browser, PHP version,
 Operating System, any installed SilverStripe modules.

Please report security issues to the module maintainers directly. Please don't file security issues in the bugtracker.

## Development and contribution
If you would like to make contributions to the module please ensure you raise a pull request and discuss with the module maintainers.
