# Code 201, 4 Jan, Read-06

## Html Tables

The **HTML  `<table>`  element** represents tabular data — that is, information presented in a two-dimensional table comprised of rows and columns of cells containing data.

```html
<table>
    <thead>
        <tr>
            <th colspan="2">The table header</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>The table body</td>
            <td>with two columns</td>
        </tr>
    </tbody>
</table>
```

## JavaScript Constructor Function

The constructor function is like "**blueprint**" for creating many objects of the same "type".

The way to create an "object type", is to use an  **object constructor function**.

Objects of the same type are created by calling the constructor function with the  `new`  keyword 

```javascript
// constructor function
function Person () {
    this.name = 'John',
    this.age = 23
}

// create an object
const person = new Person();

```

In the  example,  `function Person()`  is an object constructor function.

To create an object from a constructor function, we use the  `new`  keyword.

you can add also method to your constructor;

```javascript
// constructor function
function Person () {
    this.name = 'John',
    this.age = 23
}

// creating objects
let person1 = new Person();
let person2 = new Person();

// adding property to person1 object
person1.gender = 'male';

// adding method to person1 object
person1.greet = function () {
    console.log('hello');
}

person1.greet();   // hello

// Error code
// person2 doesn't have greet() method
person2.greet();
```

The function can be used to create multiple objects. The ```this``` keyword is used instead of the object name.
