# How to change the URL used to access the backend

By default, the backend is accessible at the `/admin` URL. This value is defined in the **prefix** option when loading the routes for HarmonyCMS.

You can change its value to meet your own requirements. Here is the default value for the admin backend:

{% code-tabs %}
{% code-tabs-item title="config/routes/harmony.yaml" %}
```yaml
_admin:
  resource: "admin"
  type: rollerworks_autowiring
  prefix: /admin
```
{% endcode-tabs-item %}
{% endcode-tabs %}

