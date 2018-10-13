# Create project

`create-project` is the command to execute to create a new HarmonyCMS project on your server.

{% hint style="info" %}
More information about this this command are available in the [Composer create-project documentation page](https://getcomposer.org/doc/03-cli.md#create-project).
{% endhint %}

When creating a new project, HarmonyFlex will perform some tasks before and after the execution of the default Composer tasks.

Consider the following example:

```bash
composer create-project harmony/skeleton my-project
```

If you execute that command, first of all Composer will create a new project from [HarmonyCMS skeleton repository](https://github.com/harmonycms/skeleton).

The first think Composer will do is loading HarmonyFlex plugin and processed like follow:

* Check connectivity to HarmonyCMS API:

![](../../.gitbook/assets/deepinscreenshot_20181012113441.png)

* Authenticate you trough our Harmony platform, using an OAuth2 Access Token
* Ask you to specify a Project ID
* Processed installing your project and all dependencies \(addons\) binded to your project
* Configure your HarmonyCMS project:
  * Updating files `.env.dist` and `.env` with project's database settings

HarmonyFlex keeps tracks of the project and addons installed in a `harmony.lock` file, which must be committed to your code repository.

