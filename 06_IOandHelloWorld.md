# IO and Hello World

---

## Programs do Input, Process, Output

Computer programs can be thought of as entities that manipulate data. It is a common concept that a program will receive data from an input device (a keyboard, a mouse, a microphone, a touchable surface, a magnetic disk - as a file or a database-, a network card, etc.), then it will process the data, and it will output this processed data to an output device (a computer screen, a headphone, a speaker, a TV, a magnetic disk - also as a file or a database-, a network card, etc.). These Input/Output devices are known as IO.

You can also consider that the input or output for a program can be another program, that can run in a different computer, and in that case you would receive input from the network card, and also output to the network card. That is how web programs work. They receive input from another program (your browser) through the network, process data, and send the output to another program (also your browser) also through the network. In this case, the output data is usually a pretty web page data. Then it is the turn of another program (guess who? Yes, your browser again) to get that web page data (as the input), process that data into a set of data representing beautifully arranged light dots (pixels), and send that processed data to an output device, your computer screen.

We will begin with a very simple IO device that has been around for many years: the console. The concept of a console is the combination of a keyboard as input, and a screen as the output. When we say a _console application_ we usually mean a program that will process text only, receiving keystrokes from the keyboard and outputting text to the computer screen. The use of a console as IO is very common, so it is also usually known as the standard input, or _stdin_, and standard output _stdout_, in many computer languages.

I Javascript, it is pretty simple to output data to the console. You have seen that you just need to use the `console.log` function. Reading from the console in Javascript is little more complicated because of its roots as a web language, but reading and writing to the console are usually among the simplest operations in most computer languages.

What can you write using console? Well, any Javascript data type. You can write numbers, or text, or other types we will learn later. For now, it is enough for you to know that the "text" data type is officially called "string", and to write literal text you need to surround it with single or double quotes. Literal number do not have quotes around them. For example:

```
console.log(123) // prints the literal number 123 on the console (screen)
console.log("this is a string") // prints the literal string "this is a string" (without the quotes) on the console
console.log('4321') // prints the literal string "4321" (without the quotes) on the console
```

One last thing to remember, when you write Javascript code: **JAVASCRIPT IS CASE SENSISTIVE!** What does it mean? It means that upper and lower case make a difference, so while `console.log('Hi')` works perfectly, `Console.log('Hi')` will cause and error because Javascript does not recognize `Console` with uppercase `C`. `console.Log('Hi')` would also cause an error for the same reason (there is no `Log` with capital `L`).

## Hello World

One famous tradition in learning computer languages is creating your first program to write the text "Hello World!" on the screen. I guess that if you have gone this far in this course you have all the knowledge you need to to that, so you are ready to do your first exercise, that you will find in the `ex01` folder, under `Exercises`: create your Hello World program and run it in Node.js.

[Back to course outline](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)

[Previous Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/05_CodeComments.md#code-comments)

[Next Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)
