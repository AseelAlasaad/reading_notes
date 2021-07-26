# Local Storage

ersistent local storage is one of the areas where native client applications have held an advantage over web applications

localStorage is a property that allows JavaScript sites and apps to save key-value pairs in a web browser.This means the data stored in the browser will persist even after the browser window is closed

 If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.

**Historically**, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data.

**they have three disadvantage of Cookies**

*  Cookies are included with every HTTP request,thereby slowing down your web application by needlessly transmitting the same data over and over.

* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet.

* Cookies are limited to about 4 KB of data — enough to slow down your application.


Microsoft invented a great many things, One of these things was called DHTML Behaviors, and one of these behaviors was called userData.


**UserData** : userData allows web pages to store up to 64 KB of data per domain

In 2007, **Google** launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers.Gears provides an API to an embedded SQL database based on SQLite. After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.


# HTML5 Storage

it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies,this data persists even after you navigate away from the web site, close your browser tab, exit your browser,Unlike cookies. this data is never transmitted to the remote web server (unless you go out of your way to send it manually).

From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object.

```html

function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage

```html 

if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}

```
**USING HTML5 STORAGE**

HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.The named key is a string.The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats.