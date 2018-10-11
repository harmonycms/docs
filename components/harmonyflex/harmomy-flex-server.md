---
description: Self hosted server for Symfony Flex allowing private and customized recipes.
---

# Harmomy Flex Server

{% hint style="info" %}
Based on the same idea as Symfony, HarmonyCMS use recipes that allow the automation of Composer packages configuration. 
{% endhint %}

### Harmony Flex server

Such as the official [Symfony Recipes server](https://flex.symfony.com), Harmony use it's own flex server to serve private recipes for each extensions and packages available through the Harmony's Marketplace. This private server is used as a proxy/caching server of the official and contrib repositories.

> This private recipes server can be accessed at the next url: [https://flex.harmonycms.net](https://flex.harmonycms.net).

{% hint style="warning" %}
This private server replace the default configured endpoint server: [https://flex.symfony.com](https://flex.symfony.com/).
{% endhint %}

### Harmony recipes repository

Like Symfony, Harmony recipes are contributed by the community and are stored in a single public repository who contains all the recipes for the extensions and packages available through the Harmony's Marketplace.

> This public repository can be accessed to the next url: [https://github.com/harmonycms/recipes](https://github.com/harmonycms/recipes)

{% hint style="info" %}
Read the [Symfony Recipes documentation](https://github.com/symfony/recipes/blob/master/README.rst) to learn everything about how to create recipes for your own packages.
{% endhint %}

