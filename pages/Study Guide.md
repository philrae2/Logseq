---
title: Study Guide
---

- Part 1: Study Guide for Test
	 - This assessment will test your knowledge of the [Prep Course](https://launchschool.com/courses/6c70a040/home) and [JS101](https://launchschool.com/courses/804d1cae/home), as well as the [Introduction to Programming with JavaScript](https://launchschool.com/books/javascript)
 book. It has a huge surface area in that it covers the JavaScript 
programming language broadly. It does not cover Object Oriented 
Programming.

- Specific Topics of Interest
	 - You should be able to clearly explain the following topics:
		 - variable scope, especially how variables interact with function definitions and blocks

		 - primitive values, objects, and type coercions
			 - primitive values
				 - [[string - datatype]]

				 - [[number - datatype]]
					 - [[NaN]]

					 - [[Infinity]]

				 - [[boolean - datatype]]

				 - [[undefined]]

				 - [[null]]

			 - ((38517cab-f68d-430c-b84b-6fc0bb3d62fb))

		 - object properties

		 - mutability vs. immutability vs. const

		 - loose and strict equality

		 - passing arguments into and return values out of functions

		 - working with Strings

		 - working with Arrays, especially the iteration methods (forEach, map, filter, find, and sort)

		 - working with Objects; accessing keys and values of an Object as arrays

		 - arrays are objects

		 - understand the concepts of __pass-by-reference__ and __pass-by-value__

		 - variables as pointers

		 - console.log vs. return

		 - truthiness vs. boolean

		 - function definition and invocation

		 - function declarations, function expressions, and arrow functions

		 - implicit return value of function invocations

		 - first-class functions

		 - side-effects

		 - naming conventions (legal vs idiomatic)

		 - be able to explain what a function does without talking about its implementation; that is, document a function's use and purpose. (See below.)

- Using a REPL
	 - JavaScript REPLs (such as Node.js) that run code as you type it do 
not run that code the same way as when you run the code from a .js file. This can lead to discrepancies in the behavior of your code. That can influence your answers on the assessment.

	 - Unless otherwise stated, all assessment questions that use code 
examples or that expect you to write code assume that the code should be
 run from a .js file. **We strongly advise against using a REPL to test the code.**

- How to Answer the Assessment Questions
	 - The questions in this assessment will typically test your knowledge and understanding at more than one level.

	 - When answering the questions, you should:

- Example
	 - Examine the code example below. The last line outputs the string 'Hi' rather than the string 'Hello'. Explain what is happening here and identify the underlying principle that this demonstrates.

	 - 
```javascript
let greeting = 'Hello';

while (true) {
  greeting = 'Hi';
  break;}

console.log(greeting);
```

	 - Compare the following possible answers to this question:

	 - A) greeting is set to 'Hello' on line 1. greeting is set to 'Hi' on line 4. Line 8 outputs greeting, which is 'Hi'.

	 - B)  The global variable greeting is assigned to the string 'Hello' on line 1. Within the loop, greeting is then reassigned to the string 'Hi' on line 4. On line 8, console.log is called with the variable greeting passed to it as an argument; since greeting is now assigned to 'Hi', this is what is output.

	 - C)  The global variable greeting is initialized to the string 'Hello' on line 1. Within the loop, lines 3 to 6 define a block within which greeting is reassigned to the string 'Hi' on line 4. On line 8, console.log is called with the variable greeting passed to it as an argument; since greeting is now assigned to 'Hi', this is what is output.

	 - D)  The global variable greeting is declared and initialized to the string 'Hello'
 on line 1. Lines 3 to 6 define a loop that will execute forever, unless
 something happens to end the loop. When the loop begins, it first 
reassigns the greeting global variable to 'Hi' on line 4. The next line, break, causes the loop to end, with execution resuming after line 6. Finally, on line 8, console.log is called with the value of the variable greeting passed to it as an argument. Since greeting is now assigned to 'Hi',
 that is what gets output. This example demonstrates variable scoping 
rules in JavaScript; specifically the fact that a variable declared in 
the outer scope is accessible from a nested inner scope.

	 - While none of these answers is technically incorrect, they all answer the question with varying degrees of detail and precision.

- Bullet Points
	 - Many students attempt to use bullet points to answer the questions on the exam. This makes sense in some situations:

	 - In short, they work well for **lists**. (Notice that we 
used a bullet list to list this list of lists!) However, they don't 
always work as complete answers for a question. You don't speak in 
bullet lists; don't write with lists.

	 - To illustrate, consider the following hypothetical explanation of the example code from the previous section:

	 - This answer is essentially a __laundry list__ of statements 
about the code. Unfortunately, laundry lists aren't very effective as 
answers on the assessment. They are difficult to follow, and often leave
 it to the reader to piece together the logic behind the list.

	 - In the above list, for instance, there's no logical progression that 
actually explains what is happening. Instead, the student has simply 
listed a bunch of statements about each line of code, plus one unrelated
 item that talks about scope. However, a program is not a series of 
independent lines of code. Code depends on what happened before, and it 
influences what happens later. There's nothing in the laundry list that 
connects those individual bits of code together.

	 - From the grader's point of view, this answer is incomplete:

	 - In short, it leaves the grader with the burden of tying your bullet points together in a coherent whole.

	 - These faults can be addressed, to a degree, in a bullet point answer.
 However, the laundry list approach often leads students to overlook 
these missing details. Paragraphs make it easier to think about the 
bigger picture since you're striving for clarity, not a list of 
everything you can think of.

	 - Some students overcompensate by listing a bunch of facts that aren't 
really pertinent to the question. For instance, a typical answer might 
list several facts about the word true above:

	 - This is mostly clutter for the grader, and there's some ambiguity 
about what "It" means in the last bullet. You may also lose some points 
if the additional details say something that is incorrect.

	 - In general, a clearly written paragraph is easier to understand and 
grade than a laundry list. While we won't penalize you for using bullet 
points, it's important to realize that bullet points have weaknesses 
that are difficult to see when you're writing.

- Precision of Language
	 - Most questions require that you explain some code with words. It's 
important to be able to describe why something happens using precise 
vocabulary and be able to pinpoint the principle (scope, shadowing, 
etc.) at work. In other words, be precise and don't be vague.

	 - For example, let's take the following piece of code.

	 - 
```javascript
let hello = "Hello, world!";function myFunc() {
  console.log(hello);}

myFunc();
```

	 - If asked to describe what the myFunc code does, you might be tempted to say:

	 - The result of the function is "Hello, world!".

	 - This statement isn't wrong, but, it's imprecise and doesn't help us 
understand the function. If you had written that as an answer, you might
 score a 2/5 on the question (40% is not a passing score).

	 - A more precise answer would be something along the lines of this:

	 - The function outputs Hello, world!, which it obtains from the global variable hello, then returns undefined. The function can use hello since functions have access to variables defined in the outer scope.

	 - In programming, we're always concerned with the output and the return
 value, as well as any object mutation and non-local variables being 
used. We need to speak in those terms, and not use vague words like 
"results."

	 - When writing answers to the test questions, be as precise as 
possible, and use the proper vocabulary. Doing this will help you debug 
and understand more complex code later in your journey. If your 
definitions are not precise, you won't be able to lean on them to 
decompose complicated code. Also, you will likely not be able to pass 
this assessment.

- Some Specifics
	 - For the purposes of this assessment, we will use some terms in very 
precise ways. You should be extremely precise in the language that you 
use as well. Doing so will prevent misunderstandings during grading. 
Relying on precise language will help both you and us understand each 
other.

	 - These areas are outlined below.

- Assignments
	 - Consider the following assignment:

	 - greeting = 'Hello';

	 - Most of the Launch School material describes this assignment as:

	 - The greeting variable is assigned to the string 'Hello'.

	 - However, there are places where we describe this code as:

	 - The string 'Hello' is assigned to the greeting variable.

	 - Both of these are acceptable in the assessment. Try to be consistent though to avoid confusion.

- Variables
	 - Unless mentioned specifically, we use the term **variable** in the broadest sense possible. On this exam, that means that all of the following should be treated as variables:

	 - Note in particular that object property names **are not** variables.

- What Code Does
	 - There are two main ways to describe the following code:

	 - function appendTo(str, otherStr) {
  for (let index = 0; index < otherStr.length; ++index) {
    str += otherStr[index];
  }

  return str;}

	 - First, there's the implementation level description. Here, we'd say something like this:

	 - We're declaring a function named appendTo that takes two arguments, both of which are presumed to be strings. We then use a for loop with an index
 local variable to iterate over the characters in the second string, 
appending each character to the value of the first string. We then 
return the result value as a new string.

	 - An implementation-level description is fine when describing the way a
 function does something. However, it's completely dependent on the 
implementation. If the implementation changes for some reason, the 
description may no longer be accurate. For instance, here's the same 
function with a completely different implementation:

	 - function appendTo(str, otherStr) {
  return str + otherStr;}

	 - The implementation-level description no longer describes this code accurately. It's not even close.

	 - That leads us to the second way to describe some code: the user-level
 description. Here, we describe what code does not how it does it. The 
description is not dependent on the implementation, but takes a 
higher-level perspective that is more enduring.

	 - appendTo is a function that takes two string arguments 
and returns a new string. The returned string contains the result of 
appending the second string to the first.

	 - Notice that we don't mention the implementation details at all. 
Instead, we provide a higher-level view of the function. There's just 
enough information that another developer can use it in their code 
without first having to understand what's going on behind the scenes.

	 - If we ask you to describe a function without reference to its 
implementation, it's this kind of user-level description that we're 
looking for. We may also ask to describe the function for other 
developers or for documentation purposes: again, we're looking for the 
user-level description.

- Truthiness
	 - In the assessment, we want you to be very clear about the distinction between __truthy__ and __falsy__ values and the boolean values true and false.

	 - In JavaScript, the __falsy__ values false, 0, NaN, "", undefined, and null are all said to __evaluate to false__ when used in a boolean context. All other values, the __truthy__ values, are all said to __evaluate to true__. Note that saying that a value evaluates to true or false is **not** the same as saying that those values **are** true or false, or that they are **equal to** true or false. These may seem like subtle distinctions, but they are important ones.

	 - Suppose we ask you to describe what is happening in this code:

	 - let a = "Hello";

if (a) {
  console.log("Hello is truthy");} else {
  console.log("Hello is falsy");}

	 - If your answer says that "a is true" or that "a is equal to true" in the conditional on line 3, we would likely deduct points from your score. A much better answer would say that "a is truthy" or that "a evaluates to true" on line 3.

	 - To sum up:

- Distinctions
	 - Be clear about the following distinctions:

- Online Resources
	 - When an online resource conflicts with Launch School materials, the 
Launch School materials should be used on the assessment. We can't grade
 assessments using information that differs from what we present, 
especially when that information is incorrectly changed.

	 - This is especially true with semi-official sources like the Mozilla 
Developer Network (MDN). Nearly anybody can update the MDN 
documentation, and those updates are sometimes incorrect.

- Additional Tips
	 - When writing code for an assessment question, run your code often to 
check it. Make sure that you have some way to run JavaScript code in 
your terminal or via an [online repl](https://repl.it/) prepared beforehand.

	 - Some Launch School students have blogged about their assessment experiences:

	 - These articles are well worth your time; don't pass them up!
