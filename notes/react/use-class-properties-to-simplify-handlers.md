# Use class properties to simplify handler functions

In JavaScript, [class methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Function/bind
) are not bound to class instances by default. In React, that means using either `.bind()` or an arrow function `onClick={(e) => this.handleClick(e)}` to pass `this`.

Alternately, use Class properties. From the React documentation:

```js
class LoggingButton extends React.Component {

	handleClick = () => {
		console.log('this is:', this);
	}

}
```
This syntax ensures that `handleClick` has the correct `this` value when called.

In some cases, properties remove the need for constructors in a class. See an example of how this works in [an article](https://medium.com/front-end-hacking/class-properties-with-react-dbc9b33e901c) by Dale Jefferson.

Originally prompted by reading [Mapbox React examples](https://github.com/mapbox/mapbox-react-examples/blob/master/data-overlay/src/index.js#L41) code.

