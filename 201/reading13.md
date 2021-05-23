# The Past, Present, and Future of Local Storage for Web Applications

HTML5 storage is a way for web pages to store key/value pairs locally in your browser. Most modern browsers now support this way to store data.

**Local Storage**: "Locally Based" - specific to your computer

**HTML5 storage** AKA _"local storage"_ or _"DOM store

Cookies are an old feature, can be used for persistant local storage of small amounts of data. They are included with every HTTP request.  
Big downsides of cookies:

- slows down web application because it repetitively transmits data
- sends unencrypted data over the internet
- limited on data size

<br>

## Check for HTML5 storage

```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

You can use Modernizr to detect support for HTML5 Storage instead of writing the function yourself:

```
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
```

## Access HTML5 storage from JavaScript with `localStorage` object

Store and retrieve data with the key name. Named key is a _string_ 

If data is not a string, use functions like `parseInt()` or `parseFloat()`


Use `getItem()` and `setItem()` to access data

```
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);

```

could be rewritten to use square bracket syntax instead:

```

var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```

To delete items:

```
interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};
```

To get the name of each key and total quantity of values in storage:

```
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};
```

<br>

[http://diveinto.html5doctor.com/storage.html]
