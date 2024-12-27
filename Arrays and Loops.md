# Basic Loops and Specialized loops
The most basic loop is the for...of loop. It takes in a collection, assigns each item in the collection to a variable name, and does something for each of them.

```javascript
const cats = ["Leopard", "Serval", "Jaguar", "Tiger", "Caracal", "Lion"];

for (const cat of cats) {
  console.log(cat);
}
```
This will just log each string to the console.

## map() and filter()
map() and filter() are more specialized types of loops. You could just use a combination of string methods and array methods to do what they do. map(), like a for...each loop, will iterate through a collection, and do something for each item. It'll then return a new collection.

```javascript
function toUpper(string) {
  return string.toUpperCase();
}

const cats = ["Leopard", "Serval", "Jaguar", "Tiger", "Caracal", "Lion"];

const upperCats = cats.map(toUpper); //map runs the toUpper function to each item in the cats collection.

console.log(upperCats);
// [ "LEOPARD", "SERVAL", "JAGUAR", "TIGER", "CARACAL", "LION" ]

```
Now you have a new collection assigned with the changed items all uppercase.

filter() on the other hand will return a new collection only if it matches conditions that you specify. 
```javascript
function lCat(cat) {
  return cat.startsWith("L");
}

const cats = ["Leopard", "Serval", "Jaguar", "Tiger", "Caracal", "Lion"];

const filtered = cats.filter(lCat);

console.log(filtered);
// [ "Leopard", "Lion" ]

```

## for vs. for...each loops

When to use which, all depends on context. If you're just trying to iterate over all of a collection's items, the for...each is fine. 

for loops are helpful if you're not necessarily iterating over a collection, but rather are just trying to perform a piece of code a bunch of times, like drawing a bunch of circles on a canvas. 

If you have a collection but have certain things you need to do to a specific item, a for loop would be better suited over a for...each since you can specify which iteration will have something done to its item.
