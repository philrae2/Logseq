---
title: NaN
---

- Not a Number is  subset of the type number in JS. It usually represents a numeric result that an error occurred or an illegal operation was attempted.

- It occurs in two situations:
	 - Undefined mathematical situations like 0 divided by 0

	 - Trying to convert a  non-number value, like a string or objects

- To determine if a number is NaN you can use two methods:
	 - 
```javascript
> let value = NaN;
> Number.isNaN(value)
= true

> Object.is(value, NaN)
= true
```
