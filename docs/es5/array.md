# ES5 Array methods

Shims for Array methods for non-ES5 compliant browsers, for instance Internet Explorer 6-8.



## Array.filter

Filter an array with a passed function.


#### Example

	array.filter(*array*, *fn*, *bind*)


	var array = require('prime/es5/array');

	array.filter([1, 2, 3], function(item){
		return (item > 1);
	});

	// returns [2, 3]



## Array.indexOf

Returns the index of an item in an array; -1 if not found.

#### Example

	array.indexOf(*array*, *item*)


	var array = require('prime/es5/array');

	array.indexOf([1, 2, 3], 2); 	// returns 1
	array.indexOf([1, 2, 3], 5);	// returns -1



## Array.map

Apply a function to all items in an array, return the mapped array

#### Example

	array.map(*array*, *fn*, *bind*)


	var array = require('prime/es5/array');

	array.map([1, 2, 3], function(item){
		return item * 2;
	});

	// returns [2, 4, 6]



## Array.forEach

Loop through an array, apply a function

#### Example

	array.forEach(*array*, *fn*, *bind*)


	var array = require('prime/es5/array');

	array.forEach([1, 2, 3], function(item){
		// do stuff
	});



## Array.every

Returns true if the whole array passes the passed function

#### Example

	array.every(*array*, *fn*, *bind*)


	var array = require('prime/es5/array');

	array.every([1, 2, 3], function(item){
		return item > 0;
	});

	// returns true

	array.every([1, 2, 3], function(item){
		return (item > 2);
	});

	// returns false



## Array.some

Returns true if some of the array passes the passed function

#### Example

	array.some(*array*, *fn*, *bind*)


	var array = require('prime/es5/array');

	array.some([1, 2, 3], function(item){
		return (item > 2);
	});