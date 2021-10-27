# Review, Research, and Discussion

**JavaScript Array map():**

The map() method creates a new array with the results of calling a function for every array element. The map() method calls the provided function once for each element in an array, in order.
map() does not change the original array.

```html
Syntax:

array.map(function(currentValue, index, arr), thisValue)
```
**JavaScript Array.reduce():**

The reduce() method executes a reducer function for each value of an array. reduce() returns a single value which is the function's accumulated result. reduce() does not execute the function for empty array elements. reduce() does not change the original array.

```html
Syntax:

array.reduce(function(total, currentValue, currentIndex, arr), initialValue)
```

**code snippets for  superagent() to fetch data from a URL and log the result With normal Promise .then()**

```html
 request
   .get('https://example.com/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });

```

**With async/await**
```html

async function () {
  try {
    var response = await request.post('/user/').send({foo: 4})
  } catch (err) {
    // do something with err...
  }
}
```

**Are all callback functions considered to be Asynchronous? Why or Why Not?**

Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. ... It iterates over each item and calls the function once per item.

##  Node Ecosystem

The JavaScript ecosystem is a collection of software packages, libraries, and other resources that facilitate development as they integrate with each other.

Node. js' package ecosystem, npm, is the largest ecosystem of open source libraries in the world.npm is the default package manager for the JavaScript runtime environment Node. js.

**CI: continuous integration**

**CD: continuous delivery**

**TDD: Test Driven Development**

TDD relates specifically to unit tests and continuous integration/continuous delivery pipelines like CircleCI, GoCD.

![CI/CD](https://miro.medium.com/max/2625/1*7RfsPZkbaaIrSs92_Dsh3w.png)