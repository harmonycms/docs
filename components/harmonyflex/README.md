---
description: >-
  Composer plugin to manage Harmony's Projects and configuration for extensions,
  packages, themes and translations.
---

# HarmonyFlex

### What is HarmonyFlex?

Based on the same idea as **Symfony Flex**, [HarmonyFlex](https://github.com/harmonycms/flex) is the _only_ way to install and manage your HarmonyCMS application.  
HarmonyFlex is a command line tool to automates installation, configuration, deployment of addons \(extensions, packages, themes and translations\) and other Composer dependencies \(default scope\).

### How does it work?

HarmonyFlex is a Composer plugin who is loaded when the user \(_you_\) execute some Composer commands. This plugin, modify the behavior of some commands such as `create-project`, `require`, `remove` and `update` by running new automated tasks to prevent the end user \(_still you_\) to perform manual actions.

To have more details on how this plugin modify the behavior of the Composer tool, check the next articles here:

* [Create project](create-project.md)
* [Require/Install](install.md)
* [Remove/Uninstall](remove.md)

{% hint style="warning" %}
We use a private proxy/caching flex recipes server, replacing as the default Symfony endpoint to install private recipes.  
For more information, read the [Harmony Flex Server documentation](../harmomy-flex-server.md).
{% endhint %}

