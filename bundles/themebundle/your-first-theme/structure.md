---
description: >-
  A HarmonyCMS theme is a set of files which you can edit in order to change
  the  look of your website.
---

# Structure

Here are a few important tidbits:

* All themes have their files located in the `/themes` folder, at the root of Harmony's folder.
* Each theme has its own sub-folder, in the main themes folder.
* Each theme is made of template files \(.html.twig\), image files \(.jpg, .png and such\), one or more CSS files \(.css\), and usually JavaScript files \(.js\).
* Each theme has a `composer.json` file, used by [Composer](https://getcomposer.org) to install it, defines all of the theme’s configuration and meta information.

Here is its organization, which is explained further below.

```text
acme
├── assets
│   ├── css
│   │   └── main.css
│   ├── javascripts
│   └── images
├── composer.json
├── translations
│   └── messages.en.yml
└── views
    ├── index.html.twig
    └── template.html.twig
```

