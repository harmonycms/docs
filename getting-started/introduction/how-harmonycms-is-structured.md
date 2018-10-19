# How HarmonyCMS is structured?

#### How HarmonyCMS is structured?

HarmonyCMS is build on top of the new reworked directory structure of Symfony 4 framework.  
We can split HarmonyCMS in 4 distinct parts, such as:

**1. CMS layer**

**2. Frameworks layer**

HarmonyCMS is based on the popular Symfony framework.

**3. Database**

**4. Directory structure**

Like explained in the next article [How to Override Symfony's default Directory Structure](https://symfony.com/doc/current/configuration/override_dir_structure.html) HarmonyCMS is automatically ships with a specific directory structure made to match what we want to achieve, to be the much simple as possible for the end user.

The HarmonyCMS default directory structure is like:

```text
    my-project/
    ├─ bin/
    │  ├─ console
    │  └─ phpunit
    ├─ config/
    │  ├─ bundles.php
    │  ├─ packages
    │  ├─ routes
    │  ├─ routes.yaml
    │  └─ services.yaml
    ├─ extensions/
    │  ├─ blocks/
    │  ├─ components/
    │  ├─ plugins/
    │  ├─ modules/
    │  └─ widgets/
    ├─ public/
    │  └─ index.php
    ├─ src/
    │  └─ ...
    ├─ themes/
    │  ├─ acme-theme/
    │  └─ ...
    ├─ translations/
    │  ├─ en/
    │  └─ ...
    ├─ var/
    │  ├─ cache/
    │  └─ log/
    ├─ vendor/
    └─ composer.json
```

