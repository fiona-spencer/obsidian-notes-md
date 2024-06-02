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
var
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

1. Length ```js ```
