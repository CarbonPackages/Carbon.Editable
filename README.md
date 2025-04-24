[![Latest Stable Version](https://poser.pugx.org/carbon/editable/v/stable)](https://packagist.org/packages/carbon/editable)
[![Total Downloads](https://poser.pugx.org/carbon/editable/downloads)](https://packagist.org/packages/carbon/editable)
[![License](https://poser.pugx.org/carbon/editable/license)](LICENSE)
[![GitHub forks](https://img.shields.io/github/forks/CarbonPackages/Carbon.Editable.svg?style=social&label=Fork)](https://github.com/CarbonPackages/Carbon.Editable/fork)
[![GitHub stars](https://img.shields.io/github/stars/CarbonPackages/Carbon.Editable.svg?style=social&label=Stars)](https://github.com/CarbonPackages/Carbon.Editable/stargazers)
[![GitHub watchers](https://img.shields.io/github/watchers/CarbonPackages/Carbon.Editable.svg?style=social&label=Watch)](https://github.com/CarbonPackages/Carbon.Editable/subscription)

# Carbon.Editable Package for Neos CMS

This package extends the Fusion prototype `Neos.Neos:ContentComponent`, `Neos.Neos:Content` and `Neos.Neos:Editable`. It is all about to toggle editability.

## Installation

`Carbon.Editable` is available via packagist. Add `"carbon/editable" : "^1.0"`
to the require section of your composer.json or run `composer require carbon/editable`.

## `Neos.Neos:ContentComponent` and `Neos.Neos:Content`

With the new property `contentElement` (default to `true`) you can turn off the content element wrapping. Great if you want to use content elements for components without any abillity to edit or inside another content element.

## `Neos.Neos:Editable`

You'll get some new features for this prototype:

| Property       | Default value               | Description                                              |
| -------------- | --------------------------- | -------------------------------------------------------- |
| `editable`     | `true`                      | Set to false if you want to disable the editable feature |
| `tagName`      | `this.class ? 'div' : null` | If this property is set, the tag is always written       |
| `innerTagName` | `null`                      | Pass an additional, inner tag inside the tagName         |
| `class`        | `null`                      | Pass a class to the tagName                              |

The already existing property `block` get a new default value: `this.tagName ? false : true`. If don't make use of the `tagName` everything stays the same.
