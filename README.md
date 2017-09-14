# Backend Challenges microservice project - package.json

Run the server.js file or view the deployed app in https://short-url-microservice.glitch.me.

* Pass a URL as a parameter and I will receive a shortened URL in the JSON response.
* If you pass an invalid URL that doesn't follow the valid http://www.example.com format, the JSON response will contain an error instead.
* When you visit that shortened URL, it will redirect you to the original link.

## Example creation usage:

```js
https://short-url-microservice.glitch.me/new/https://www.google.com
```

## Example creation output:

```js
{"original_url":"https://www.google.com","short_url":"https://short-url-microservice.glitch.me/3502"}
```

## Usage:

```
https://short-url-microservice.glitch.me/3502
```

### Will redirect to:

```
https://www.google.com/
```

N.B it is used a mLab mongodb database. there are this env variables:

```
MONGOLAB_URI=mongodb://test:test@ds038547.mlab.com:38547/url-shortener
APP_URL=https://short-url-microservice.glitch.me/
```