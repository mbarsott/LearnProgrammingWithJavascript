# Code Comments

---

When you write programs, it is sometimes useful to write comments, so you, or anyone reading the program, can understand it better. 

The comments are completely ignored by the program interpreter in the computer, so you can write anything on the comments and it will never cause any error.

In Javascript there are two types of comments: line comments and block comments.

A line comment starts when the program reaches the two forward slashes in sequence. This informs the computer that whatever follows those slashes in that line is a comment and should not be considered program instructions. For example:

```
// This is a comment. The entire line is ignored by the computer when running the program.
console.log(23) // This prints the number 23 on the console. Anything after the slashes is a comment.
```

As you can see above, line comments can be used on lines that contain Javascript code. Anything from the slashes to the end of the line is ignored.

A block comment is anything between the characters `/*` and `*/`. It can appear anywhere in a Javascript program and can span multiple lines. For example:

```
/* This is a Javascript block comment.
   This comment spans more than one line. */
/*
   Anything between "whack asterisk" and "asterisk whack" is not considered actual Javascript code, and is ignored
   when running the program.
*/
console.log(/*The answer to the fundamental question, according to a certain book*/42) // prints 42
```
As you can see above, you can mix and match both types of comments.

Comments are used to explain code, call attention to parts of the program, inform about licenses and copyrights, and they can also be used to organize your thoughts before writing a program: you can write the pseudocode for your program as comments and then add the actual Javascript commands or replace the comments with commands to implement the pseudocode.

You will see this in this course exercises. The exercises are contained in numbered folders under the `exercises` folder. Every exercise is one or more files that contains instructions as comments. For example, this is exercise number one (file `HelloWorld.js` in the `ex01` folder):
```
// Write a program that prints the string "Hello, World!" using the console.log function
// You should write your code in place of the comment below that reads // place your code here
// The program below should produce the following output:
// Hello, World!

// place your code here
```
In this case all you have to do is replace the last comment line with your code. Try doing this and running the program using Node.js.

[Back to course outline](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)

[Previous Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/04_BasicStructuresAndPseudocode.md#basic-programming-structures-and-pseudocode)

[Next Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)
