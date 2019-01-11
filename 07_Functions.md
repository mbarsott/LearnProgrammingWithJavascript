# Functions

---

A sequence of computer program instructions to perform a specific task, packaged as a unit, is called a _subroutine_. In Javascript you create subroutines using functions. There are many reasons to write your code in functions. Among them:  

1. you can organize your code in smaller parts, that are easier to understand on their own;  
2. you can reuse the function over and over again and from multiple places (for example, `console.log` is a function you will use many, many times throughout this course);  
3. you can isolate parts of your code from others, making it harder to introduce unwanted errors. 

To create functions in Javascript you have to write the keyword `function` followed by one or more spaces, the name of your function, a list of parameters between parenthesis, and your code between curly braces. For example, let's say you frequently want to write the current date and time to your console, so you know when the output was generated. You could write a function like this one:

```
function printWithDateAndTime() {
   var now = new Date();
   console.log(now);
}
```

Woah, too much information! Ok, let's break it down and talk a little about coding in Javascript in general.

First, as in any language, there are some _keywords_. These are special words that have a specific meaning in the programming language and cannot be used for anything else in the program. In the example above, `function` and `var` are Javascript keywords. If you type them in an editor with syntax highlight, they will appear in a different color, so you can spot keywords from miles away. 

Second, there are spaces. When you write Javascript, just like in English for the most part, you have to separate words using spaces, and you use spaces before or after certain symbols (or punctuation) to make your code or text more readable. Specifically in Javascript, the characters `space`, `tab`, and `new line` (or `carriage return` or `enter`) are all considered "spaces". In some places spaces are required, for example to separate words, and in others they are optional. Wherever you can use one space, you can also use many spaces. For example if you have three tabs followed by one new line and then by five spaces, Javascript will treat all these characters the same way it would treat one single space. You can use this to make your code more readable, and we will see some space conventions used to make code prettier.

Third, you can create your own names for some Javascript elements. In the example above we create our own name for the function, `printWithDateAndTime`, and for one variable, `now` (we will talk about variables in another part of the course). These names are used to identify the elements you create (like your variables and your functions), so they are called identifiers. Identifiers start with one character but they cannot contain spaces (otherwise Javascript would undrestand it as more than one word, and consequently more than one identifier, because spaces are used to separate words in the language). So, in order to make your spaceless names more readable, we use the convention of starting every following English word in the identifier with a capital letter. That is why, in our example, the words "With", "Date, "And", and "Time", all start with a capital letter. Notice how it is easy to read `printWithDateAndTime` even though there are no spaces between the words. If the very first word in the identifier starts with a lowercase letter we say we are using the camel case convention, for example, "calculateLivesLeft". If the first word starts with an uppercase letter, we say we are using Pascal case convention. Most Javascript style guides recommend using camel case for your identifiers.

Fourth, there are some paired symbols, like parethesis `( )` and curly braces `{ }`. These pairs are used to contain lists of other elements. For example we will learn that parenthesis can contain a list of parameters to a function, and curly braces can contain a list of Javascript code statements. Curly braces containing Javascript code are very important, and we call them a code block. In the example above you have the following code block:

```
{
   var now = new Date();
   console.log(now);
}
```

Fifth, you may have noticed a semicolon after each Javascript statement. It serves to inform the computer that the statement ended. It is like a period in English sentences. You could even put two statements in the same line if you use the semicolon at the end of each one, but your code will be a lot more readable if you write one statement per line, so this is considered a best practice.

Most of the very popular computer languages require that you have all your code contained in subroutines, or functions, and have a way to identify which one is the very first that should be executed, the program "entry point". Javascript is a little unconventional in the sense that there is no specific entry point in a java program. If you load a Javascript program in an execution environment, like node.js, or a web page, the execution environment will go top to bottom, trying to execute everything it finds. That is why our very first program Hello World, was just a console.log statement in a text file. As soon as node.js finds a loose statement, it executes it.

Functions, on the other hand, need to be called in order to be executed. You have seen that in order to define a function you use the keyword `function` followed by the function name. Javascript will not execute the statements defined in the function unless you execute the function. In order to execute, or call, the function, in any other part of the program, you just write the function name, followed by parenthesis and the list of arguments you want to pass to the function parameters (we will talk about parameters and arguments ahead). If there are no arguments, you just use the parenthesis. So, for example, to call the function we defined above, we would write the following statement:

```
printWithDateAndTime();
```

So, for example, if you load the following program in node.js (or Plunker), nothing will happen, because it is just a function definition, and the function is never executed:

```
function printWithDateAndTime() {
   var now = new Date();
   console.log(now);
}
```

But if you load the following program, it will print the current date and time (using Universal, or UTC, time), because not only the function is defined in the program, but it is also executed (called) right below its definition:

```
function printWithDateAndTime() {
   var now = new Date();
   console.log(now);
}

printWithDateAndTime();
```

Well I guess you now have the knowledge needed to try the second exercise, under the [`Exercises/ex02` folder](https://github.com/mbarsott/LearnProgrammingWithJavascript/tree/master/Exercises/ex02).

## Returning values

A function can return a value to it's caller. This is done with the keyword `return`. Whenever javascript finds the keyword return it will stop executing the function and return to the point where the function was called. If the keyword `return` is followed by an expression, the result of the expression will be the value returned by the function. Try the following code in node.js:

```console.log(returnTitle())
console.log(returnHello());
console.log(returnWorld());
console.log(returnNothing());

function returnTitle() {
    return 1;
}

function returnHello() {
    return 'Hello';
}

function returnWorld() {
    return 'World';
}

function returnNothing() {
    return;
}
```


 [Back to course outline](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)

[Previous Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/06_IOandHelloWorld.md#io-and-hello-world)

[Next Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)
