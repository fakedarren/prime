# Number



## limit

number.limit(*number*, *min*, *max*)

number.limit(5, 1, 3); // returns 3


## round

number.round(*number*, *precision*)

number.round(3.1415)		// returns 3
number.round(3.1415, 2)		// returns 3.14


## times

number.times(*number*, *fn*)

number.times(3, function(i){
	alert(i + '!');
});

alerts '1!', '2!', '3!'


## random

number.random(*max*)

number.random(3) // returns a number between 1 and 3