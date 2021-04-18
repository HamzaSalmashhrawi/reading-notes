# Intro & scripts

### ACCESS CONTENT
#### You can use JavaScript to select any element, attribute, or text from an HTML page. For example:
* Select the text inside all of the <hl> elements on a page
* Select any elements that have a c 1 ass attribute with a value of note
* Find out what was entered into a text input whose id attribute has a value of ema i 1 


### MODIFY CONTENT
#### You can use JavaScript to add elements, attributes, and text to the page, or remove them. For example:
* Add a paragraph of text after the first <hl> element
* Change the value of c 1 ass attributes to trigger new CSS rules for those elements
* Change the size or position of an <i mg> element


### PROGRAM RULES
#### You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page. For example:
* A gallery script could check which image a user clicked on and display a larger version of that image.
* A mortgage calculator could collect values from a form, perform a calculation, and display repayments.
* An animation could check the dimensions of the browser window and move an image to the bottom of the viewable area (also known as the viewport). 

### REACT TO EVENTS
#### You can specify that a script should run when a specific event has occurred. For example, it could be run when:
* A button is pressed
* A link is clicked (or tapped) on
* A cursor hovers over an element
* Information is added to a form
* An interval of time has passed
* A web page has finished loading

## A SCRIPT IS A SERIES OF INSTRUCTIONS
#### A script is a series of instructions that a computer can follow to achieve a goal. 
### To write a script, you need to first
#### state your goal and then list the tasks that need to be completed in order to achieve it. 

#### Start with the big picture of what you want to achieve, and break that down into smaller steps. 
### 1. DEFINE THE GOAL 
#### First, you need to define the task you want to achieve. You can think of this as a puzzle for the computer to solve.
### 2. DESIGN THE SCRIPT
#### To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle. This can be represented using a flowchart. You can then write down individual steps that the computer needs to perform in order to complete each individual task (and any information it needs to perform the task), rather like writing a recipe that it can follow.
### 3. CODE EACH STEP
#### Each of the steps needs to be written in a programming language that the compu ter understands. In our case, this is JavaScript.

# EXPRESSIONS
### An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions. 
#### 1. EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE 
##### In order for a variable to be useful, it needs to be given a value. As you have seen, this is done using the assignment operator (the equals sign).
* var color = 'beige';
##### The value of co 1 or is now beige. When you first declare a variable using the var keyword, it is given a special value of undefined. This will change when you assign a value to it. Technically, undefined is a data type like a number, string, or Boolean.

# Functions:
### WHAT IS A FUNCTION?
#### Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). 
### A BASIC FUNCTION
##### 
#### Before the closing </body> tag, you can see the link to the JavaScript file. The JavaScript file starts with a variable used to hold a new message, and is followed by a function called updateMessage(). 
#### You do not need to worry about how this function works yet - you will learn about that over the next few pages. For the moment, it is just worth noting that inside the curly braces of the function are two statements

### Function expressions
#### While the function declaration above is syntactically a statement, functions can also be created by a function expression.

#### Such a function can be anonymous; it does not have to have a name. For example, the function square could have been defined as:

* const square = function(number) { return number * number }
var x = square(4) // x gets the value 16

#### However, a name can be provided with a function expression. Providing a name allows the function to refer to itself, and also makes it easier to identify the function in a debugger's stack traces:

 * #### const factorial = function fac(n) { return n < 2 ? 1 : n * fac(n - 1) } console.log(factorial(3))
#### Function expressions are convenient when passing a function as an argument to another function. The following example shows a map function that should receive a function as first argument and an array as second argument.

### Calling functions
#### Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

#### Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:

