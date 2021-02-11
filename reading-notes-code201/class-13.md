# Code 201, 11th Jan, Read-13

## Local Storage in JavaScript

Basically **local storage** is the storage of data locally without using any **php** or other languages or any services, but only using JavaScript and **inside the web browser**  and in more formal way:

### Local Storage Property

`localStorage` is a property that allows JavaScript sites and apps to save key/value pairs in a web browser with no expiration date. This means the data stored in the browser will persist even after the browser window is closed.

## Local Storage Access

you can access the local storage property from the _**Window**_ object.
you can access it in two way :

```javascript
window.localStorage
```

```javascript
localStorage
```

## Storage Object

if you ```console.log``` the ```localStorage``` it will actually give what is called **Storage Object**

## Method for Storage Object

if you check the  prototype of Storage object you will see the following method.

```javascript
Storage.clear() // empty the storage
Storage.getItem() 
Storage.key()
Storage.removeItem()
Storage.setItem()
```

* The **`clear()`** method of the `Storage` interface clears all keys stored in a given `Storage` object.

* The **`getItem()`** method of the `Storage` interface, when passed a key name, will return that key's value, or `null` if the key does not exist, in the given `Storage` object.

* The **`key()`** method of the `Storage` interface, when passed a number n, returns the name of the nth key in a given `Storage` object. The order of keys is user-agent defined, so you should not rely on it.

* The **`removeItem()`** method of the `Storage` interface, when passed a key name, will remove that key from the given `Storage` object if it exists. The **`Storage`** interface of the Web Storage API provides access to a particular domain's session or local storage.
* The **`setItem()`** method of the `Storage` interface, when passed a key name and value, will add that key to the given `Storage` object, or update that key's value if it already exists.
* The **`length`** read-only property of the `Storage` interface returns the number of data items stored in a given `Storage` object.

[My GitHub Page](https://omar-tarawneh.github.io/reading-notes/class-13)
