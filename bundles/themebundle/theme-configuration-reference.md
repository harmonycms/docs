# Theme configuration reference

**theme**

**type**: `string` **default**: `default`  
The theme used to render the frontend pages.

{% code-tabs %}
{% code-tabs-item title="theme.yaml" %}
```yaml
harmony:
  theme: 'default'
```
{% endcode-tabs-item %}
{% endcode-tabs %}

#### Templating

The ThemeBundle provides a number of functions to use in templates.

**Twig Extensions**

| Twig Function | Templating Helper | Arguments | Explanation |
| :--- | :--- | :--- | :--- |
| `asset_theme` | _getThemeUrl_ | string $path, string $packageName = null | A Twig function to get assets from a theme path. |
| `asset` | _getAssetUrl_ | string $path, string $packageName = null | Override default function, check asset exists in current active theme, otherwise fallback to original path. |

| Twig Filter | Templating Helper | Arguments | Explanation |
| :--- | :--- | :--- | :--- |
| `theme` | _getThemeUrl_ | string $path, string $packageName = null | A Twig filter to get assets from a theme path. |

**Global Variables**

| Variable Name | Explanation |
| :--- | :--- |
| `harmony.site_name` | Get the site name defined in the parameter's file _harmony.yaml_ |

