# Introduction

1. You need a valid access token to send requests to the API endpoints. You can get one in the [API Access](https://account.harmonycms.net/settings/api) section in your account's settings.
2. Response to every request is sent in [JSON format](https://en.wikipedia.org/wiki/JSON). In case the API request results in an error, it is represented by an `"error": {}` key in the JSON response.
3. The request method \(verb\) determines the nature of action you intend to perform. A request made using the `GET` method implies that you want to fetch something, and `POST` implies you want to save something new, and so on for the other ones.
4. The API calls will respond with appropriate [HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes) for all requests. A `200 OK` indicates all went well, while `4XX` or `5XX` response codes indicate an error from the requesting client or our API servers respectively.



