# FizzBuzz JS

Simple solve for FizzBuzz in Javascript.

```javascript
var replace = [ {"number" : 3, "word" : "fizz"}, {"number" : 5, "word" : "buzz"} ] ; //things to replace
for(var i = 1; i <= 100; i++){ //loop from 1 to 100
	var output = "" ; //what will come out
	for (var j = 0; j < replace.length; j++){ //loop through replace
		if (i % replace[j].number == 0){ //if current number 'i' divided by number in 'replace at j' has no remainder
			output = output + replace[j].word //output is current state of output with the new word on the end
		}
	}
	if (output.length == 0){ //if output isn't changed by above code output the current number 'i'
		output = i //output is current number
	}
	console.log(output) //log the output
}
```