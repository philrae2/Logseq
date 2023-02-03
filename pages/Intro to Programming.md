---
title: Intro to Programming
---

- Data Types
	 - In most of your code, you should use the capitalized name when you're referring to a built-in feature of JavaScript. The one exception to this rule is with the typeof operator -- it always returns a lowercase string value, so typeof 3 returns "number".

	 - A [[literal]] is any notation that lets a fixed value be represented in the source code.
		 - Examples are:
			 - 
```javascript
'Hello, World!' //string literal
3.1245 //number literal
{a: 1, b:2} // object literal
undefined //undefined
```

	 - [[string - datatype]]

	 - [[number - datatype]]

	 - [[boolean - datatype]]

	 - [[undefined]]

	 - [[null]]

- Operators
	 - An operator is **capable of manipulating a certain value or operand** or data types that javascript has.
 Operators are used to perform specific mathematical and logical 
computations on operands. In other words, we can say that an operator 
operates the operands. In JavaScript operators are used for compare 
values, perform arithmetic operations etc.
		 - An operator is word that is able to manipulate values/operands/data types in JavaScript like the math operators of addition. The addition operator will work on two operands or values to find their sum.

- Coercion
id:: 38517cab-f68d-430c-b84b-6fc0bb3d62fb
	 - Explicit Coercion 
		 - Is when you are deciding what variable type you will be changing to. We can use Number("12"), String(43), numberVariable.toString()

		 - Numeric Coercion
			 - Number()
				 - Number will coerce a string to a number if the string has a valid numeric value, but not a combination of valid and invalid characters

				 - When we try to coerce a variable that doesn't contain valid numeric characters JS will not throw an error and instead return NaN. JS will fail silently
					 - 
```javascript
> Number('foo')
= NaN
```

			 - parseInt()
				 - ParseInt() will convert a string to a number but only up to whole numbers and will ignore non-numeric characters.
					 - 
```javascript
> parseInt('12xyz')
= 12
```

					 - 
```javascript
> parseInt('3.1415')
= 3
```

			 - parseFloat()
				 - parseFloat() will convert a string containing  decimal numeric characters to a decimal number type

				 - 
```javascript
> parseFloat('12.5foo')
= 12.5
```

		 - String Coercion
			 - String()
				 - We can coerce numeric values to strings

				 - 
```javascript
> String(20)
= '20'
```

	 - Implicit Coercion occurs when the JavaScript Engine chooses how the variable will be changed. 

- Data Structures
	 - Arrays
		 - Arrays is one of the two most common data structure in JS. 

		 - Arrays can contain strings, numbers, objects, or any other data type

		 - The array indexes must be non-negative numbers

	 - Objects
		 - Are the second most common type of data structure in JS. 

		 - They differ from arrays in that their index are automatically coerced as strings compared to arrays where their indexes must be non-negative numbers
