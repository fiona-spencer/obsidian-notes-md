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

## If Statements

```js
function trueOrFalse(isTrue){
	if(isTrue){
		return "YES, TRUE";
	}
	return "NO, FALSE";
}
```

## Equality Statements
1. Non-strict (\==)
2. Strict (\=\==)
3. Inequality (!=)
4. Strict inequality (!\==)

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