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

You can create Javascript programs using any text editor. Javascript program files have the extension `.js`. You can create a program that prints the result of the expression `2+1` and run it from node. In order to do that, use a text editor to create a file `exp.js` containing the following Javascript statement (we will learn about statements, and expressions, and the console later, in the course): ```console.log(2+1)```

To execute the program, open the Command Prompt or Terminal on the folder containing the file, and type: ```node exp.js[Enter]```

You should see the result 3 printed out. You could have written just the expression `2+1`, and node would evaluate it, but not print it, like the REPL did. The actual Javascript command to print things on the screen (or console, in this case), is `console.log()`.

## Plunker

---

You can access the Plunker website at [plnkr.co](https://plnkr.co). I recommend creating a user in Github, if you do not have one yet, and then using your Github user to Sign in to Plunker. Creating a Github user is free, and there is a `Sign in with Github` button on the top right corner of most Plunker screens. If you are signed in, you can save your Plunks (projects) and go back to the point you left in the future.

On the Plunker home page, there is a button that reads `Launch the Editor`, and this will take you to the web page where you can edit your files. By default you will get a Plunk that contains a web page, `index.html`, a readme file `README.md`, a Javascript file `script.js`, and a CSS file `style.css`. These files are listed on the left side of the screen and you can check their contents by clicking on each one of them.

On the top right side of the page there is the icon of an eye. You click that icond to "see" your website on the right panel. The default Plunk is a web site that displays the phrase "Hello Plunker!". You can type your Javascript code on the `script.js` file, and everything is already hooked up for your code to execute. If you click on the `script.js` file name, on the left panel, you can see it contains the following text: 

```// Code goes here```

Replace that content witht he Javascript print statement we used previsouly, when we ran a program in Node:

```console.log(2+1)```

You may be disappointed for not seeing the result right away, but believe me, it is there. To see the printed result of your Javascript program, you have to check the browser "Console". In Chrome you can go to the menu, select `More tools` and then `Developer tools`, or press `[Ctrl+Shift+I]` or `F12`. The Developer Tools pane will appear, and then you can click on 'Console' to see what is printed there. Many things will be already written on the Console, but the result of the expression, `3`, should be the last one. The reason for other things showing up on the Console, is that the browser Console is presenting information that comes from the entire page, that means the Plunker website page, and not only from your program. In addition to that, Plunker works in a way that every change you make on your Plunk is evaluated and displayed, so you may see partial results of the code you typed in your program, including errors if the Javascript command was evaluated before you finished typing.

You can enter a name for your Plunk on the "Description" text area on the left panel, under "PLUNK", and if you made changes to your Plunk you can save them with the `Save` button on the top toolbar. If you leave Plunker and return another day, after you login with your Github user, you can click on your user name on the top right, and from the drop down menu select "My plunks" to see all your saved Plunks. When you move your mouse pointer over any of these Plunks, the very first icon, "Edit this Plunk" will take you back to the Plunk editor, at the point you last saved your work.

## Integrated Development Environment

---

I mentioned you can write your Javascript programs in any text editor, and that is true. It does not mean it is wise, though. If you use an Integrated Development Environment, or IDE, that understands Javascript, your life will be A LOT easier when creating or editing your  programs. You will probably get many benefits like syntax highlighting, auto completion, and many others, and you will be able to find your errors a lot quicker. There are many nice IDEs available for free, but I usually recommend sticking to the most popular technologies, instead of the coolest ones, although sometimes they are the same. The reason for that is twofold: first, if it is popular, there is a high demand for people with that skill; second, the technology is a lot less likely to die. That being said, the most popular IDE on the Stackoverflow developers survey, 2018, is Visual Studio Code, which is a wonderfull free tool, written in Electron with Javascript by the Microsoft folks, and runs on Windows, Mac, and Linux. If you prefer using other IDE, there is Atom and Sublime for free, or Webstorm for a fee, or any other tool you prefer. Really, I will not dig into IDEs here, and using one is just a suggestion. 

If you want to install and learn about Visual Studio Code you can do it from the official [Visual Studio Code website](https://code.visualstudio.com/).

[Back to course outline](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learnprogrammingwithjavascript)

[Previous Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/02_WhyJavaScript.md#why-javascript)

[Next Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learnprogrammingwithjavascript)
