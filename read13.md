### What is HTML5 Storage?

It's a way for web pages to store named (key/value) pairs locally, within the client web browser. this data persists even after you navigate away from the web site, close your browser tab, or even exit the browser, This data is never transmitted to the remote web server (Unless you sent them manually).

### Which browser?

Well, the latest version of pretty much every browser supports HTML5 Storage… even Internet Explorer!

| browser | version |
| :-----: | :-----: |
|   IE    |  8.0+   |
| Firefox |  3.5+   |
| Safari  |  4.0+   |
| Chrome  |  4.0+   |
|  Opera  |  10.5+  |
| iPhone  |  2.0+   |
| Android |  2.0+   |

### Check for HTML5 Storage.

You can run this code in your console to check f your browser support the HTML Storage.

```javaScript
if (Modernizr.localstorage) {
  // window.localStorage is available!
  console.log("Supported");
} else {
    console.log("Not Supported");
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
```

## Using HTML5 Strorage.

HTML5 Storage is based on named (key/value) pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

Like other JavaScript objects, you can treat the localStorage object as an associative array, you can use "dot notation" or "brackets notation", we have multiple methods such as

- setItem(key,value).
- getItem(key).
- removeItem(key).

If you called getItem() method and gave it a key that is not exist in localStorage, it will return null.

if you calles removeItem() method and gace it a key that is not exist in localStorage, it will do nothind
