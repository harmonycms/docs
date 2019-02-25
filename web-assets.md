# Web Assets

Web assets are things like CSS, JavaScript and image files that make the frontend of your site look and work great.  
In your HarmonyCMS application there are bound to exist many **assets** either created by you or provided by third-party \(extensions, bundles or themes\).

As part of your deploy procedure, you have to use some Symfony **console** command to actually make the assets available to the frontend of your application.

## assets:install

This command is available in Symfony core, no extra bundle is required. So this is probably the first you should get to know.  
It will search through all available bundles for a **/Resources/Public/** folder and copy the content into `public/bundles/{bundle-name}/`.

```bash
php bin/console assets:install
```

## extension:assets:install

This command is provided by the [HarmonyExtensionBundle](https://dev-docs.harmonycms.net/bundles/extensionbundle).  
It will search through all available extensions for a **/Resources/Public/** folder and copy the content into `public/extensions/{extension-name}/`.

```bash
php bin/console extension:assets:install
```

## theme:assets:install

This command is provided by the [HarmonyThemeBundle](https://dev-docs.harmonycms.net/bundles/themebundle).  
It will search through all available themes for a **/Resources/Public/** folder and copy the content into `public/themes/{theme-name}/`.

```bash
php bin/console extension:assets:install
```

