# Make an enum-like structure

Enums help document intent. To create an enum-like structure in JavaScript, you can use the Object.freeze method.

Example:

```javascript
const COLORS = {
	red: "#CE0C0C", 
	green: "#00F0B5", 
	blue: "#26547C"
};

Object.freeze(COLORS);

console.log(COLORS.red); // #CE0C0C
```

See this discussion on [Stack Overflow](https://stackoverflow.com/questions/287903/what-is-the-preferred-syntax-for-defining-enums-in-javascript).
For more discussion on Enums, see this [thread](https://stackoverflow.com/questions/4709175/what-are-enums-and-why-are-they-useful). TypeScript supports [Enums](https://www.typescriptlang.org/docs/handbook/enums.html) natively.