# HarmonyFlex

{% hint style="info" %}
Based on **Symfony Flex**, [HarmonyFlex](https://github.com/harmonycms/flex) is the _only_ way to install and manage your HarmonyCMS application.  
HarmonyFlex is a tool to automates installation, configuration, deployment of addons \(extensions, packages, themes and translations\) and other Composer dependencies.
{% endhint %}

#### How does HarmonyFlex work?

HarmonyFlex is a Composer plugin that modifies the behavior of the `create-project` command.  
When creating a new project, HarmonyFlex will perform some tasks before and after the execution of the default Composer tasks.

Consider the following example:

```bash
composer create-project harmony/skeleton:dev-master project
```

If you execute that command, first of all Composer will create a new project from [HarmonyCMS skeleton repository](https://github.com/harmonycms/skeleton).  
After that, HarmonyFlex will make some requests to the HarmonyCMS API server to:

1. Authenticate you using an OAuth2 Access Token,
2. Will ask you to specify a Project ID,
3. Will processed installing your project and all dependencies \(addons\) binded to your project,
4. Will configure your HarmonyCMS project.

HarmonyFlex keeps tracks of the project and addons installed in a `harmony.lock` file, which must be committed to your code repository.

