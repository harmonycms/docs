# Require/Install

HarmonyFlex register to the `post-package-install` event, who occurs after the package is installed and performs some tasks when predefined package types are loaded by Composer.  
Here is the details about the different supported package types when Composer require/install a dependency.

### Themes

They are identified by the [Composer type](https://getcomposer.org/doc/04-schema.md#type) `harmony-theme` who install the theme to the next location: `themes/${name}`.

### Translations

They are identified by the [Composer type](https://getcomposer.org/doc/04-schema.md#type) `harmony-translation` who install the translation to the next location: `translations/${name}`.

