*This repository is a mirror of the [component](http://component.io) module [kewah/css-animation-event-types](http://github.com/kewah/css-animation-event-types). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/kewah-css-animation-event-types`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# css-animation-event-types

CSS animation event types detection. Adds vendor prefix if the browser is not compliant.  

## Installation

    $ component install kewah/css-animation-event-types

## Example

```
var cssAnimEventTypes = require('css-animation-event-types');
 
if(cssAnimEventTypes.start !== undefined) {
  var foo = document.getElementById('foo');
  foo.addEventListener(cssAnimEventTypes.start, onAnimStart, false);
  foo.addEventListener(cssAnimEventTypes.iteration, onAnimIteration, false);
  foo.addEventListener(cssAnimEventTypes.end, onAnimEnd, false);
} else {
  console.log('CSS animation not supported');
}
```

   

## License

  MIT
