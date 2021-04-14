# How do i write a script for a web page
### HOW HTML, CSS, & JAVASCRIPT FIT TOGETHER 
#### Before diving into the JavaScript language, you need to know how it will fit together with the HTML and CSS in your web pages.
* HTML
   * This is where the content of the page lives. The HTML gives the page structure and adds semantics.

  
* CSS
   * The CSS enhances the HTML page with rules that state how the HTML content is presented (backgrounds, borders, box dimensions, colors, fonts, etc.). 


* JavaScript
   * This is where we can change how the page behaves, adding interactivity. We will aim to keep as much of our JavaScript as possible in separate files. 


![imgdif](https://www.onely.com/wp-content/uploads/blog/2020/Ultimate_Guide_JS_SEO_2020_Edition/003-chapter1-html-css-js-chart-1000x563.jpg)



## CREATING A BASIC JAVASCRIPT
#### JavaScript is written in plain text, just like HTML and CSS, so you do not need any new tools to write a script. This example adds a greeting into an HTML page. The greeting changes depending on the time of day. 

## JAVASCRIPT RUNS WHERE IT IS FOUND IN THE HTML
#### When the browser comes across a <script> element, it stops to load the script and then checks to see if it needs to do anything.  

## Basic JS instructions 
#### A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon. 
#### A script is a series of instructions that a computer can follow one by one. Each individual instruction or step is known as a statement. Statements should end with a semicolon. 

### Notes
* Each of the lines of code in green is a statement.
* The pink curly braces indicate the start and end
of a code block. (Each code block could contain many more statements.)
* The code in purple determines which code should run (as you will see on p149). 

### A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

#### When you write JavaScript, you have to tell the interpreter every individual step that you want it to perform. This sometimes involves more detail than you might expect. Think about calculating the area of a wall; in math the area of a rectangle is obtained by multiplying two numbers: width x height = area  . You may be able to do calculations like this in your head, bu t when writing a script to do this calculation, you need to give the computer very detailed instructions. You might tell it to perform the following four steps in order:

1. Remember the value for width
2. Remember the value for height
3. Multiply width by height to get the area
4. Return the result to the user 



## DATA TYPES
#### JavaScript distinguishes between numbers, strings, and true or false values known as Booleans

* NUMERIC DATA TYPE The numeric data type handles numbers:
  * For tasks that involve counting or calculating sums, you will use numbers 0-9. For example, five thousand, two hundred and seventy-two would be written 5272 (note there is no comma between the thousands and the hundreds). You can also have negative numbers (such as -23678) and decimals (three quarters is written as 0.75) 
* STRING DATA TYPE The strings data type consists of letters and other characters.
   * Note how the string data type is enclosed within a pair of quotes. These can be single or double quotes, but the opening quote must match the closing quote. Strings can be used when working with any kind of text. They are frequently used to add new content into a page and they can contain HTML markup. 

* BOOLEAN DATA TYPE Boolean data types can have one of two values: true or false.
  * It might seem a little abstract at first, but the Boolean data type is actually very helpful. You can think of it a little like a light switch - it is either on or off. As you will see in Chapter 4, Booleans are helpful when determining which part of a script should run.


## variables
### RULES FOR NAMING VARIABLES
1. The name must begin witha letter, dollar sign ($),or an underscore (_). It must not start with a number
2. The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name.
3. You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something. For example, var is a keyword used to declare a variable. Reserved words are ones that may be used in a future version of JavaScript. ONLINE EXTRA View a full list of keywords and reserved words in JavaScript.
4. All variables are case sensitive, so score and Score would be different variable names, but it is bad practice to create two variables that have the same name using different cases.
5. Use a name that describes the kind of information that the variable stores. For example, firstName might be used to store a person's first name, l astNarne for their last name, and age for their age.
6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word. For example, f i rstName rather than firstnarne (this is referred to as camel case). You can also use an underscore between each word (you cannot use a dash). 






