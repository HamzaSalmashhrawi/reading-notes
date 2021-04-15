# Logical operators
#### There are four logical operators in JavaScript: || (OR), && (AND), ! (NOT), ?? (Nullish Coalescing). Here we cover the first three, the ?? operator is in the next article.

#### Although they are called “logical”, they can be applied to values of any type, not only boolean. Their result can also be of any type.
#### There are four logical operators in JavaScript: || (OR), && (AND), ! (NOT), ?? (Nullish Coalescing). Here we cover the first three, the ?? operator is in the next article.

## Comparison operators: Evaluating condtions:

#### you can evaluate a situation by comparing one value in the script to what you expect it might be. the result will be a boolean: true or false
## example on Comparison operators:

### Comparison operators are usually used on numeric or date fields, but can also be used on text fields:

#### 1. >greater than.

#### 2. >= greater than or equal to.

#### 3. < less than

####/ 4. <= less than or equal to

#### 5. = is equal to

#### 6. <> is not equal to

Arithmetic operators
Arithmetic operators perform math operations:

#### 1. +for addition

#### 2. – for subtraction

#### 3. – (unary) changes a negative number to a positive number

#### 4. * multiplies two numbers

#### 5. / divides numbers

#### 6. \ divides the first value by the second value and rounds to the nearest integer

## Logical operators: 

## JavaScript Loops
#### Loops are handy, if you want to run the same code over and over again, each time with a different value. Often this is the case when working with arrays

### Different Kinds of Loops
### JavaScript supports different kinds of loops:
### but in this read the loops included just (for) and (while):
* for - loops through a block of code a number of times

* while - loops through a block of code while a specified condition is true
### for loop:
#### Statement 1 is executed (one time) before the execution of the code block.

#### Statement 2 defines the condition for executing the code block.

#### Statement 3 is executed (every time) after the code block has been executed.

### While Loops
##### The while loop loops through a block of code as long as a specified condition is true.

##### It writes out the 5 timestable. Each time the loop is run, another calculation is written into the variable called msg. This loop will continue to run for as long as the condition in the parentheses is true. That condition is a counter indicating that, as long as the variable i remains less than 10, the statements in the subsequent code block should run. Inside the code block there are two statements: The first statement uses the+= operator, which is used to add new content to the msg variable. Each time the loop runs, a new calculation and line break is added to the end of the message being stored in it. So+" works as a shorthand for writing: msg = msg + 'new msg' (See bottom of the next page for a breakdown of this statement.) The second statement increments the counter variable by one. (This is done inside the loop rather than with the condition.) When the loop has finished, the interpreter goes to the next line of code, which writes the msg variable to the page.