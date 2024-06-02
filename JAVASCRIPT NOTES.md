## Comments

```js
var sum = 10 + 10;   //in-line comment
/*
multi-line comments
*/
console.log(sum);
```

## Data Types

```js
var myName;   //undefined
var myName = null;   //null
var positive = false;   //boolean
var myName = 'Fiona';   //string
var myName = 'A';   //symbol
var myNumber = 3;   //number
var arr = [1, 2, 3, 4] //array with indexes
var myObj = {
	"name" : "fiona",
	"age" : 21,
	"height" : 180
};   //object with properties
```

## Math Operations

* addition (+)
* subtraction (_)
* multiplication (*)
* division (/)
* modulus (%)
* increment (++)
* decrement (--)

## Assignment Variables

```js
var a;  //declaration
var b = 2;  //declaration and assignment
```

## Incrementing

```js
var myVar = 10;
myVar++;  //equivalent to myVar = myVar + 1;
myVar--;  //equivalent to myVar = myVar - 1;
//Augmented math operations
myVar+= 5;
myVar-= 5;
myVar*= 5;
myVar/= 5;
```

## Escaping Sequences

```js
var myStr = "I am a \"double quoted" string inside";
```

* \\b - backspace
* \\t - horizontal tab
* \\n - newline
* \\v - vertical tab
* \\f - form feed
* \\r - carriage return
* \\" - double quote
* \\' - sing quote
* \\ - backslash
* \\Xnn - The Unicode character specified by the two hexadecimal digits nn
* \\Unn - The Unicode character specified by the four hexadecimal digits nnnn
* \\U {n} - The Unicode character specified by the code point n, where i is one to six hexadecimal digits between 0 and 10FFFF (ES6)

## Quoting Strings

```js
var myStr = `<a href="https://google.com>" target"_blank>LINK</a>`;
```

## String Concatenation

```js
var first = "My name is ";
var second = "fiona";
var totalString = first + second;
```

## String Properties

1. Length 
```js
var lastName = "Spencer;
var lastNameLength = lastName.length;
```

## Zero-Based Indexing

```js
var myStr = '123';
var first = myStr[0];  //1
var first = myStr[1];  //2
var first = myStr[2];  //3
```

## String Character Immutability

```js
myStr[0] = "H";   //does not work, instead
myStr = "Hello";
```

## Arrays

```js
var arr = ["John", 23];
var multiArr = ["Smith", [1, 2, 3], ['A', 'B']];
```

## Modify Arrays

```js
var myArray = [1, 2, 3, 4, 5];
myArray[0] = 10;
```

## Access Multi-Dimensional Array

```js
myArray[2][1] = "C";
```

## Manipulating Arrays
1. Push
2. Pop
3. Shift
4. Unshift


```js
var arr = [1, 2, 3];
arr.push(4);   //[1, 2, 3, 4]
arr.pop();     //[1, 2, 3]
arr.shift();   //[2, 3]
arr.unshift(0) //[0, 2, 3]
```

## Functions

```js
function test(){
	console.log("Hello, world!");
}

var sum = 0;

//undefined function
function addThree(){
	sum = sum + 3;
}

//defined function
function addFive(){
	return sum += 5;
}
```

## Function with Arguments

```js
function test(parameter1, parameter2){
	console.log(parameter1 + parameter2);
}

test();
```

## Scope
1. Global
2. Local

## nextInLine Function
```js
function nextInLine(arr, item){
	arr.push(item);
	return arr.shift();
}

var testArr = [1, 2, 3, 4, 5];

console.log("Before :" + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6));
console.log("After :" + JSON.stringify(testArr));
```

## If/Else-if Statements

```js
function trueOrFalse(isTrue){
	if(isTrue){
		return "YES, TRUE";
	}
	return "NO, FALSE";
}

function requirement(age){
	if (age > 18){
		return "allowed";
	} else if (age < 18){
		return "denied";
	} else if (age == 18){
		return "you are 18"'
	} else {
		return "please enter a number";
	}
}
```
## For Loop

```js
var ourArray = [];

for (var i = 0; i < 5; i++){  //inital, condition, increment
	ourArray.push(i);
}

//nested for-loops

function addAll(arr){
	var result;

	for (var i = 0; i < arr.length; i++){
		for (var i = 0; i < arr[i].length; i++){
			result += arr[i][j];
		}
	}
	return result;
}

var values = addAll([1, 2, 3], [4, 5], [6]);
```
## While Loop

```js
var myArray = [];

var i = 0;
while(i < 5){
	myArray.push(i);
	i++;
}

console.log(myArray);
```

## Do While Loop

```js
var myArray = [];
var i = 10;

do {
	myArray.push(i);
	i++;
} while (i < 5)

console.log(i, myArray);  //11, [10]
```

## Switch Statements

```js
function caseInSwitch(val){
	var answer = "";
	switch(val){
		case 1:
			answer = "alpha";
			break;
		case 2:
			answer = "beta";
			break;
		case 3:
			answer = "gamma";
			break;
		case 4:
			answer = "delta";
			break;
	}
	return answer;
}

console.log(caseInSwitch(1));

function characterSwitch(val){
	var answer = "";
	switch(val){
		case "a":
			answer = "apple";
			break;
		case "b":
			answer = "banana";
			break;
		case "c":
			answer = "cat";
			break;
		default:
			answer = "please enter again";
			break;
	}
	return answer;
}

console.log(characterSwitch(1));
```

## Equality Statements
1. Non-strict (\==)
2. Strict (\=\==)
3. Inequality (!=)
4. Strict inequality (!\==)
5. Greater than (>)
6. Greater than or equal to (>=)
7. Less than (<)
8. Less than or equal to (<=)

```js
function testEqual(val){
	if (val == 12){
		return "Equal";
	}
	return "Not Equal";
}

/* strict type comparison
3 === 3 - true
3 === "3" - false
*/
```

## And/Or Operations
1. &&
2. ||

## Returning Boolean

```js
function isLess(a, b){
	return a < b'
}

isLess(10, 15);
```

## Objects

```js
var ourDog = {
	"name": "camper",
	"legs": 4,
	"tails": 1,
	"food": ["chicken", "beef"]
};
```

## Accessing Objects
1. Dot notation
2. Bracket notations
```js
var testObj = {
	"hat": "ballcap",
	"shirt": "jersey",
	"shoes": "cleats",
	"a pair of socks": "white"
};

var hatValue = testObj.hat;
var shirtValue = testObj.shirt;

var sockValue = testObj["a pair of socks"];
var clothingType = "";
var clothingValue = testObj[clothingType];
```

## Adjusting Objects

```js
var ourDog = {
	"name": "camper",
	"legs": 4,
	"tails": 1,
	"food": ["chicken", "beef"]
};

//changing property
ourDog.name = "Emma";
//adding a new property
ourDog.bark = "woof";
ourDog['toy'] = "sheep";
//deleting a property
delete ourDog.bark;
```

## Object Lookup

```js
function phoneticLookup(val){
	var result = "";
	var lookup = {
		"alpha": "Adams",
		"bravo": "Boston",
		"charlie": "Chicago",
		"delta": "Denver",
		"echo": "Easy",
		"foxtrot": "Frank"
	};
	result = lookup[val];
	return result;
}

console.log(phoneticLookup("charlie"));
```

## Testing Objects

```js
var myObj = {
	gift: "pony",
	pet: "kitten",
	bed: "sleigh"
};

function checkObj(checkProp){
	if (myObj.hasOwnProperty(checkProp)){
		return "contains property: " + myObj[checkProp];
	} else {
		return "not found, please enter another property";
	}
}

console.log(checkObj("gift"));
```

## Complex Objects

```js
var myMusic = [
	//First record
	{
		"artist": "Billy Joel",
		"title": "Piano Man",
		"release_year": 1973,
		"format": [
			"CD",
			"LP"
		],
		"favourites": false
	},
	//second record
	{
		"artist": "Elton John",
		"title": "Yellow Brick Road",
		"release_year": 1973,
		"format": [
			"LP"
		],
		"favourites": true
	}
];


//accessing nested objects
var myStorage = {
	"car": {
		"inside": {
			"glove box": "maps",
			"passenger seat": "bag"
		},
		"outside": {
			"trunk": "spare tire"
		}
	}
};

var gloveBoxContents = myStorage.car.inside.["glove box];
```

## Random Function

```js
function randomNumber(min, max){
	return Math.floor(Math.random90 * (max - min + 1)) + min;
}

randomNumber(0, 10);  //range 0-10, exlusive
```

## Math Objects

1. Math.abs
2. Math.PI
3. Math.sin
4. Math.cos
5. Math.tan
6. Math.min
7. Math.max
8. Math.pow
9. Math.exp
10. Math.sqrt
11. Math.log
12. Math.ceil
13. Math.floor
14. Math.round
15. Math.random
16. Math.trunc

## Parsing

```js
function convertToInteger(str){
	return parseInt(str);
}

function convertToBinary(str){
	return parseInt(str, 2);  //argument, base
}

convertToInteger("60");
convertToBinary("1010");
```

## Ternary Operator

```js
//conditon ? statement-if-true : statement-if-false
function checkSign(sum){
	return num > 0 ? "positive" : "negative";
}
checkSign(10);

//nested ternary
function checkAge(age){
	retrun age > 18 ? "enter" : age < 18 ? "denied" : "you are 18';
}
checkAge(18);
```