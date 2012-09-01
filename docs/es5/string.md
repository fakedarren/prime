# ES5 String methods

Shims for String methods for non-ES5 compliant browsers, for instance Internet Explorer 6-8.


## String.trim

Trims a string. Duh.


#### Example

	string.trim(*string*)


	var string = require('prime/es5/string');

	string.trim('    foo  ');

	// returns 'foo'