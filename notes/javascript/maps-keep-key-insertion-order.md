# Maps keep key insertion order and are iterable

In contrast to how plain JavaScript objects do not maintain keys in insertion order, the [ES6+ Map data type](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map#Objects_and_maps_compared#Objects_and_maps_compared) does keep insertion order of keys. 

Usefully, they are also directly iterable with a forEach method on their prototype. Adapted from [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map/forEach):

```js
function logMapElements(value, key, map) {
  console.log(`m[${key}] = ${value}`);
}


const myMap = new Map([
 	[
      "first", 1
    ],
   	[
      "second", 2
    ],
   	[
      "third", 3
    ],
 ]).forEach(logMapElements);


/* Output:
	"m[first] = 1"
	"m[second] = 2"
	"m[third] = 3"
*/

```