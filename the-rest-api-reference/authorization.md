# Authorization

{% hint style="info" %}
An **OAuth2 token** is required to be sent as part of some requests to the HarmonyCMS API, in the form of an `access_token` in the request URL or header.  
Requests that require authentication will return `401 Unauthorized`.
{% endhint %}

### **OAuth2 token \(sent in a header\)**

```bash
curl -H "Authorization: token OAUTH-TOKEN" https://api.harmonycms.net
```

### **OAuth2 token \(sent as a parameter\)**

```bash
curl https://api.harmonycms.net/?access_token=OAUTH-TOKEN
```

### Request access token

```bash
curl -X GET \
  'https://api.harmonycms.net/oauth/v2/token?client_id=CLIENT_ID&client_secret=CLIENT_SECRET&grant_type=password&username=USERNAME&password=PASSWORD' \
  -H 'Cache-Control: no-cache'
```

#### **Required parameters**

* **client\_id** - The resource owner's client id.
* **client\_secret** - The resource owner's client secret.
* **grant\_type** - Must be set to the value password.
* **username** - The resource owner's user name.
* **password** - The resource owner's password.

> `client_id` and `client_secret` are used to identify the current user \(you\) to the REST API and deliver an authenticated `access_token`.

#### Returns

This request will returns by example:

```javascript
{
    "access_token": "Y2U3YWRmMTRjZGMzMjEwMWJmOGVlOWM2NGQ4Njc3NGE1YjIwMTVjODc3NDFiOGZlZWIzZTBjZWE3ZmQyMDU3Yw",
    "expires_in": 3600,
    "token_type": "bearer",
    "scope": null,
    "refresh_token": "MWQwZWE1NjY3ODM0ZTE1YTUzOThiMzhlYTY5MjQ3ZTgyZjYyNmMyZTRlZWQ4OTY0NTFjNjg3NzkwYmU5Y2Y4NQ"
}
```

> You will find a list of all requested access token in the [API Access](https://account.harmonycms.net/settings/api) section of your account's settings.

### Root endpoint

You can issue a `GET` request to the root endpoint to get all the endpoint categories that the REST API supports:

```bash
curl https://api.harmonycms.net
```

### API Reference

Full HarmonyCMS REST API documentation car be found in the [API](https://developer.harmonycms.net/api) section of the developer part of HarmonyCMS website.

