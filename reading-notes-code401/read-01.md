# Read-01, Code 401, 24 Mar 2021

```javascript
Array.map();
```

Loop through each element of the array, process it with callback function and return the new in elements in new Array;

```javascript
Array.reduce();
```

return one value, which is called the Accumulator which been processed using the callback function that been called once for each element;

# Superagent

Example 1(using then & catch):

```javascript
function getLatAndLon(cityName) {
  superagent
    .get(url)
    .then((data) => {
      let lat = data.body.latt;
      let lon = data.body.long;
      console.log(lat, lon);
    })
    .catch((error) => {
      console.error(error);
    });
}
```

Example 2 (using async and await):

```javascript
async function getLatAndLon (cityName) {
	let data = await superagent.get(url);
	let lat = data.body.latt;
	let lon = data.body.long;
	console.log(lat, lon):
}
```

## Promises

There are three states of Promise in JavaScript

- pending
- Resolved
- Rejected

Pending which mean that the code need some amount of time to get done,
if the time is fulfilled then it's maybe Resolved or Rejected, it will be resolved if the there is no errors occurred for any reason and Rejected if there is any error or anything didn't meet the requirements;

## Callback Functions

**Are all callback functions considered to be Asynchronous?**
simply are NO;
**Why?**
Because, callback functions are regular functions when you call them and mostly they are synchronous function, and if you want to know if a certain function is asynch or synch read the documentation for it :);

[gitHub-Link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code301/read-01)
