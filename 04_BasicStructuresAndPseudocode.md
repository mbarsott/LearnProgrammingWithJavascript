# Basic Programming Structures and Pseudocode

---

There are many types of algorithms, and many ways to develop and describe them. We will stick to the basics here so we will be using pseudocode, which is a high level description of a problem solution or algorithm, in language that is close to English. For general purpose algorithm description, it is common to use Structured English, but the pseudocode style can be adapted to get close to the target computer language that will be used. The big difference is that a program is intended to be read by a computer, while a pseudocode is intended to be read and understood by human beings.

While you gain experience, and for bigger or complex problems, it is very common to write down a pseudocode version of the algorithm before trying to write it down directly in a computer language. It helps to keep your ideas clear and break down the problem in smaller and simpler chunks, without having to deal with details and particularities of a specific formal computer language. Some people prefer using diagrams, like flowcharts, but for the description of algorithms, and for the purpose of this course, we will be using Structured English, because I can write it directly in my IDE as comments, and when I am satisfied with the overall solution, I can include the actual code by replacing or adding to the comments I have already written.

There are only three categories of Structured English elements:
1. Operation statements are written as English imperative phrases and executed from top down:  

```print name```    
```set balance to 0```    
```read email address```

2. Conditional blocks, indicated by keywords like "if", "then", "else", "end if", etc.:
```
if balance < -1000  
then  
   freeze customer checking account
else 
   execute checking account transaction
end if
```  
 
3. Repetition blocks, indicated by keywords like "while", "do", "until", etc.:  
```
while there are unprocessed customers do
   get next customer
   print customer checking account statement
end while
```

We will look into each of the Structured English keywords when we learn their Javascript equivalents. One important thing to notice here is that in Structured English you are not bound by strict rules. You can adapt the style of your pseudocode as you gain more experience and you target it to a specific language. For example, you learned that in order to print in Javascript you can use `console.log()`. If you, and the people you are communicating to, understand it, you can perfectly use `console log name` instead of `print name` in your pseudocode. Also, as you learn new language conditional or repetition blocks, feel free to use them in your Structured English pseudocode. For example, if you learn about a `for each` repetition statement in your target computer language, and it feels clear what it means, you could replace the last block above by  
```
for each customer in get next customer
   print customer checking account statement
end for each
```

Another important thing is that you can refine and detail the operations statements to the point they can be easily implemented in a computer language. For example, the `print customer checking account statement` above, can be something very complicated, and you may need another algorithm to define just that. So that statement, in reality, is the execution of another algorithm, or, as in many computer languages, the execution of a separate "function". For example:
```
function print customer checking account statement (customer)
   get customer data for statement header
   print statement header
   get customer transactions for the last month
   order transactions in ascending transaction date order
   get customer balance before last month
   for each transaction in customer transactions
      calculate new balance
      print transaction line and new balance
   end for each
   print statement footer
end function
```
And then, of course you can refine and detail statements further and further in new functions. This is one of the most important skills you can learn when creating algorithms and computer programs. Experience will teach you how to think generically about a problem solution, in large abstract steps, and then refine and detail each step successively until you can implement your program in a computer language.

Also notice that inside blocks, no matter if conditional, repetition, of function blocks, the code inside the block is indented, so you can easily see what is inside and what is outside of that block.

[Back to course outline](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)

[Previous Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/03_ExecutionAndDevelopmentEnvironments.md#execution-and-development-environments)

[Next Page](https://github.com/mbarsott/LearnProgrammingWithJavascript/blob/master/README.md#learn-programming-with-javascript)
