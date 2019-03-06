---
description: This article describes how to install HarmonyCMS in your system.
---

# Installation

## Initiating a new HarmonyCMS project

To create your new HarmonyCMS project, first make sure to fulfill the [requirements](../reference/requirements/) and have [Composer](https://getcomposer.org) installed. If you don't, start by [_installing Composer globally_](https://symfony.com/doc/current/setup/composer.html) on your system.

Now, create your new HarmonyCMS project by running:

```php
composer create-project harmony/skeleton:dev-master my-project
```

This will create a new `my-project` directory, download all needed dependencies into it and generate the basic HarmonyCMS structure directories and files you'll need to have a complete functional project. In other words, your new new website will be ready!

### Memory limit errors <a id="memory-limit-errors"></a>

Installation may sometimes fail on some commands with this message:

```text
PHP Fatal error: Allowed memory size of XXXXXX bytes exhausted <...>
```

In that case, see the [Memory limit errors](https://getcomposer.org/doc/articles/troubleshooting.md#memory-limit-errors) page for Composer.

