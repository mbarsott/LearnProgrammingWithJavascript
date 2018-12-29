# Execution and Development Environments

---

We have seen that Javascript is the language of the web, and it can run on every major modern browser. In addition to that, depending
on the framework used, it can run on Windows, Mac OS/X, Linux, tablets, smartphones and probably a bunch of other places too. 

In order to keep things simple, we will limit the number of execution environments. We will use an environment that allows Javascript to
run as a server (or desktop application) on Windows, Mac, and Linux, but since one of the big strenghts of Javascript is running on
browsers, we will also have a taste of that too.

To run Javascript in a "standalone application" context, we will use Node.js. Node.js is a JavaScript runtime, designed to build network
applications, like web server ones. It is a very popular open source platform that can run on Windows, Mac, and Linux. So popular, i
n fact, that on the Stackoverflow Developer Survey of 2018, Node.js is the most popular option in the "Framework, Library, or Tool" 
category.

To run Javascript on a web browser, we will use a web site that is a combination of development and execution environment: Plunker. On Plunker you can create your own web projects, or "_plunks_", containing your Javascript code that will run on browsers, together with whatever other files are needed for that, like _HTML_ and _CSS_ files. Feel free to use Plunker from any browser you want, but I will only provide instructions for the most common one, Google Chrome. If you use other browser, like Firefox, Edge, or Safari, you will have  to find the equivalent commands on your own, but hey, this can be a good thing: you learn to program and also increase your web search and problem solving skills, all at once.

## Node.js

---

To run Node.js you have to first download it and install it. You can obtain the most recent version for your computer at the official website [nodejs.org](https://nodejs.org). Use all the defaults for the installation. If you are running on Linux you may need to do some research on the Internet about how to get Node properly installed, but if that is the case, you are certainly already used to doing that.

You can verify that node was properly installed by opening the Command Prompt on Windows (type `[Windows key]`, `cmd`, and `[Enter]`), or the Terminal Application on Mac or Linux, and then typing `node --version[Enter]`. If a version number comes up on the screen, you are good.

If you type `node[Enter]` you will see the Node REPL prompt, `>`. REPL stands for Read, Evaluate, Print, Loop. The prompt indicates that Node will _Read_ whatever expression you type. It can be a Javascript expression or a REPL command. Then the REPL will _Evaluate_ the expression you typed, _Print_ the result of the expression, and _Loop_ back to the _Read_ step. For example, if you type `2+1[Enter]`, Node will show the result of the expression, `3`, and will go back to the prompt. If you want to exit the REPL you can type the command `.exit`.

If you type something the REPL considers it needs to keep reading to evaluate, the REPL will present `...`, and you may think you are stuck, because no matter what you type you keep getting the `...` back. In that case, press `[Ctrl+C]` or type the command `.break` to go back to the REPL prompt. The command `.help` presents the REPL valid commands.

You can create Javascript programs using any text editor. Javascript program files have the extension `.js`. You can create a program that prints the result of the expression `2+1` and run it from node. In order to do that, use a text editor to create a file `exp.js` containing the following Javascript statement (we will learn about statements, and expressions, and the console later, in the course):

```console.log(2+1)```

To execute the program, open the Command Prompt or Terminal on the folder containing the file, and type:

```node exp.js[Enter]```

You should see the result 3 printed out. You could have written just the expression `2+1`, and node would evaluate it, but not print it, like the REPL did. The actual Javascript command to print things on the screen (or console, in this case), is `console.log()`.

## Plunker

---

Yadda yadda yadda

[Back to course outline](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learnprogrammingwithjavascript)

[Previous Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/02_WhyJavaScript.md#why-javascript)

[Next Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learnprogrammingwithjavascript)
