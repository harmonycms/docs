# How HarmonyCMS is structured?

#### How HarmonyCMS is structured?

HarmonyCMS is build on top of the new reworked directory structure of Symfony 4 framework.  
We can split HarmonyCMS in 4 distinct parts, such as:

## **CMS layer**

This layer is on top of everything, it represent the final product, here HarmonyCMS.  
  
The CMS layer add specific features who defined what is a CMS. It helps the final end user to manage his website the simple as possible to a non-developer user.  
In this layer we will find some graphic interfaces to manage the whole site, such as settings, extensions and themes management.

This CMS layer is decoupled in multiple bundles:

* [CoreBundle](https://github.com/harmonycms/core-bundle): provide the main features for HarmonyCMS,
* [ThemeBundle](https://github.com/harmonycms/theme-bundle): provide a theme management system,
* [WebProfilerBundle](https://github.com/harmonycms/web-profiler-bundle): profiler bundle adding debug information about HarmonyCMS environment.
* [MenuBundle](https://github.com/harmonycms/menu-bundle): provide a menu management system,
* [ExtensionBundle](https://github.com/harmonycms/extension-bundle): provide an extension management system.

## **Frameworks layer**

The framework layer's most basic responsibility is allowing individual software components to communicate. In HarmonyCMS case, the framework layer is represented by the Symfony 4 framework.  
****This framework has been chosen for these particular reasons:

1. **Reputation**: stable environment that is both well-known and recognized internationally,
2. **Permanence**: use the latest and fastest version of PHP,
3. **Flexibility**: powered by bundles to expand and reuse functionalities,
4. **Resources**: great and big community, comprehensive and detailed documentation which is extremely useful for newbies and experienced developers as well.

## **Database**

Since Symfony doesn't provide a component to work with the database, but provide a tight integration to a third-party library, you will need to work with [Doctrine DBAL](https://www.doctrine-project.org/projects/dbal.html).  
  
HarmonyCMS will not be shipped with any Doctrine component because it will not only support ORM databases \(MySQL, PostgreSQL, ...\) but ODM databases such as MongoDB will also be supported.

## **Directory structure**

Has explained in the next article [How to Override Symfony's default Directory Structure](https://symfony.com/doc/current/configuration/override_dir_structure.html) HarmonyCMS is automatically ships with a specific directory structure made to match what we want to achieve, to be the much simple as possible for the end user.

The HarmonyCMS default directory structure is like:

```text
    my-project/
    ├─ bin/
    │  ├─ console
    │  └─ phpunit
    ├─ config/
    │  ├─ bundles.php
    │  ├─ extensions.php
    │  ├─ packages
    │  ├─ routes
    │  ├─ routes.yaml
    │  ├─ services.yaml
    │  └─ themes.php
    ├─ extensions/
    │  ├─ harmony/
    │  │  └─ acme-demo/
    │  └─ ...
    ├─ public/
    │  └─ index.php
    ├─ src/
    │  └─ ...
    ├─ themes/
    │  ├─ harmony/
    │  │  └─ acme-theme/
    │  └─ ...
    ├─ translations/
    │  ├─ en/
    │  └─ ...
    ├─ var/
    │  ├─ cache/
    │  └─ log/
    ├─ vendor/
    │  └─ ...
    └─ composer.json
```

