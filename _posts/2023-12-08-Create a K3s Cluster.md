---
layout: post
title:  "Check if the objects within an array list contain the search value - Javascript"
categories: Javascript
tags: frontend js array object javascript
---

Sometimes we might not want to perform a search in the API service that gathers data from the database because it'd take a little longer for the response from server.

Just doing a quick search in the client-side (front-end) within the array list of objects resolves the problem.

```js

const itemsList = [
    {name: 'Rafael', car: 'Audi'}, 
    {name: 'John Doe', car: 'BMW'}, 
    {name: 'Ezio', car: 'Ferrari'}
    ]

const hasMatches = (obj, str) => {
    return Object.values(obj).filter(s => s.toString().match(new RegExp(str, 'i'))).length > 0
}

console.log(itemsList.filter(item => hasMatches(item, 'Rafael'))) 
// 0: [{name: 'Rafael', car: 'Audi'}]

console.log(itemsList.filter(item => hasMatches(item, 'Doe')))
// 0: {name: 'John Doe', car: 'BMW'}
```
 - `itemList`: Contain array of objects.
 - `obj`: Object with the values. 
 - `hasMatches()`: Function that checks if the object contains the value. Return true or false according to the length condition.
 - `Object.values()`: Return an array with properties values.
 - `filter()`: ES6 built-in function which returns the object that meets the criteria.
 - `match(new RegExp(str, 'i'))`: Js built-in function that uses the Regex to check if it has any matches even if the value is Mayus or Minus.
 - `toString`: Converts the entry value to a string type.


