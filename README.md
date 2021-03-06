# Native Facebook SDK login for Meteor (v1.7+) with Graph API V3.2

<a href="https://www.repostatus.org/#active"><img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed." /></a>

This package use [cordova-plugin-facebook4](https://www.npmjs.com/package/cordova-plugin-facebook4)

Documentation of the Cordova plugin [here](https://www.npmjs.com/package/cordova-plugin-facebook4)

## Install - n/a via NPM

```
meteor npm install meteor-facebook-login
```

## Setup

- Requirements:

```
meteor add http
meteor add cordova:cordova-plugin-facebook4@3.1.0 (or latest)
```

- Setup cordova plugin (mobile-config.js):

```js
App.configurePlugin('cordova-plugin-facebook4', {
    APP_NAME: 'Name',
    APP_ID: '000000000000'
});
```

## Use

(Server)

```js
import 'meteor-facebook-login';
```

(Client)

```js
import { FB_API } from 'meteor-facebook-login';

// Login with Facebook
FB_API.login(function(err) {
    if (err) {
        console.log(err);
    } else {
        console.log('login...');
    }
});
```

Also tested with IOS 12, cordova-ios 4.5.5, cordova 8.1.1, cordova-android 7.1.1



## License
MIT
- 
