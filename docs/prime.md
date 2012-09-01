# Prime


#### Example

var Animal = prime({
	
	constructor: function(age){
		this.age = age;
	}

});

var Cat = prime({
	
	implement: Animal,

	constructor: function(name, age){
		this.parent.age = age;
		this.name = name;
	}

});


var fluffy = new Cat(2, 'Fluffy');

console.log(fluffy.age);
console.log(fluffy.name);