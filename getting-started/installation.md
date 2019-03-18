---
description: This article describes how to install HarmonyCMS in your system.
---

# Installation

## 1. Initiating a new HarmonyCMS project

To create your new HarmonyCMS project, first make sure to fulfill the [requirements](../reference/requirements/) and have [Composer](https://getcomposer.org) installed. If you don't, start by [_installing Composer globally_](https://symfony.com/doc/current/setup/composer.html) on your system.

Now, create your new HarmonyCMS project by running:

```php
composer create-project harmony/skeleton:dev-master my-project
```

This will create a new `my-project` directory, download all needed dependencies into it and generate the basic HarmonyCMS structure directories and files you'll need to have a complete functional project. In other words, your new new website will be ready!

{% hint style="info" %}
Installation may sometimes fail, see troubleshooting for the [Memory limit error](https://docs.harmonycms.net/reference/troubleshooting#memory-limit-errors)
{% endhint %}

## 2. Database installation

HarmonyCMS is currently supporting SQL and No-SQL databases. To do that, this CMS is fully decoupled from any database system. **This means, you will have to choose between SQL and No-SQL.**

Such has Symfony, HarmonyCMS doesn't provide a component to work with the database, but it _does_ provide tight integration with a third-party library called [Doctrine](http://www.doctrine-project.org/).

### SQL

```bash
composer require symfony/orm-pack
```

{% hint style="info" %}
Full documentation available in the [Databases and the Doctrine ORM](https://symfony.com/doc/current/doctrine.html) Symfony page.
{% endhint %}

### No-SQL

```bash
composer require emulienfou/mongodb-pack
```

{% hint style="info" %}
Full documentation available in the [DoctrineMongoDBBundle](https://symfony.com/doc/current/bundles/DoctrineMongoDBBundle/index.html) Symfony page.
{% endhint %}

