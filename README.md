<details>
 <summary> week 1 </summary>
 
# Introduction to Python
 
 * the introduction of using commands and how to navigate them
 * learnt how to apply the syntax of python
  
# Variables and Operators, data structure
  
* apply how to use different variables within python, such int, floats and decimal numbers
* got familier with the use of output variable to produce the task performed, such as normally used variable print()
* the application of true or false value, which is another variable in python
* data structures to asign mutliple variables
* the use of dictionaries by doing some exercises 
* the use of arithmetic operation to perform calculations
* the operators on strings, the use of operator to add two strings
* Completed some exercises to test myself how to narvigate with these different operators 
* got to learn about boolean values (True or False)

# Lists, Sets, Dictionaries and Tuples
  
* learnt how lists are used to store multiple items in a single variable using square brackets [ ]
* A set is a collection which is unordered, unchangeable, and unindexed. they using 
* also got to do some exercises to test myself how to list items in a variable
* learnt about dictionaries on how they are constructed and applied using curly { }, and they have keys and values
* learnt about tuples how they are differentiated from sets and lists using different brackets, for tuples we use curly brackets ()

# Methods that are used in python

* learnt how to use different methods such as
* remove() to remove from the list
* pop() to remove the specified index 
* del also remove specified index
* clear() emptied the list
* 
# Control flow (if , elif and else statements)

* got to learn how if statements are constructed to check the condition
* got to learn of "elif" keyword which is used if previous conditions were not true
* also got to learn how "else" keyword function to catches anything that is catched by preeciding conditions
* accessing tuple by using indexing format

# Loops 

* learnt how loops are used in python to execute statements
* With the while loop we can execute a set of statements as long as a condition is true
* with for loop i learnt that you can execute sets of statements
* With the continue statement we can stop the current iteration, and continue with the next
* With the break statement we can stop the loop even if the while condition is true
* the importance of using inreament while looping to avoid the loop continuing forever

# Factorials

* learnt that the factorial represented by a exclamation mark after a number
* also that is equal to the product of that number, all the integers below it to one
* also learnt that is important to check the input
* factorial can be used to check the variable type

# Functions 

* in python a function is defined using "def" keyword
* example: def my_function() 
* to call a function, use the functiopn name followed by parentheses
* The function body is indented and contains the code that performs the desired operation on the inputs, and the "return" keyword is used to specify the output
* a function may mutate a variable without returning anything
* Functions can take one or more arguments, and they may or may not return a value
* the special Python keyword "None" represents the absence of value, and it is the default return value for functions that do not explicitly return anything

# Classes and Objects

* when we define a class, we use an uppercase letter fintor the class name, and we start defining all the functions and attributes inside the class definition
* we usually begin by creating a special function called the initialization function, or "init" function, which gets called every time an instance of the class is created
* almost everything in Python is an object, with its properties and methods
* a Class is like an object constructor, or a "blueprint" for creating objects

# Int and Floats

* python automatically returns a float to accomodate non-whole numbers
* adding a float to an int or multiplying or using exponents

# Alternative number types(Decimal, Booleans and Strings)

* if you pass a second argument as a number it will convert the first argument as a number, it will convert the first argument from thaat base to base 10.
* learnt that if you pass a second argument as a number, it will convert the first argument from that base 10. for instance "100" in base 2 is equal to 4 in base 10
* also got to know that the first argument must always be a string, even if want to convert it from different base
* this is done because there may be non-numeric characters in the string that are valid in some bases
* learnt that python has another class decimal that addresses some of the issues we saw with floats
* got to understand that floats are great they have floating point errors that can be problematic in certain situations, such as when dealing money.
* to use use decimal module, you need to import the decimal class and the getContext function at the top of your code
* the getContext function returns a context object that holds global settings for using decimal class.
* with deciaml class you can instatiate a decimal object with a number value, for instance decimal 1 devided by decimal 3 returns 0,3333 with four deciaml places
* You can also pass in a float, but be aware that the decimal module will try to exactly replicate the float with all its digits, which may lead to floating point errors
* python easily casts integers to booleans -1 is true and 0 is false, anything except 0 is true
* in fact anything except 0 is true, so even -1 amd imaginary 1 are true, but float 0 imaginary 0 are false
* string is true, anything other than an empty string is also true
* the only false string is an empty one, but be careful not to accidentally have a space in there
* we can also cast data structures to booleans, an empty list or dictionary is false
* python has numerous tools to analyze and construct strings, and one of the most useful is slicing
* slicing refers to taking a portion of a string and returning it

# Formatting

* python has a few ways to create strings, including string concatenation and f-strings
* f-strings allows us to insert variable or expressions inside curly braces in a string
* we can also do rounding and number formatting with f-strings
* the format fuction is similar to f-strings and was used in vertions of python 3.6

# Multiple-line strings

* python has a handy feature for creating multi-line strings by using triple quotes.
* if we to include literal triple quotes in the string, we can escape them with backlash.
 
</details>
<details>
 <summary> Week 2 </summary>

# Functions

* we call the function performaOperation with two parameters to determine the sum by using the operation "sum"
* to address this we can assign a default value to the operation parameter using name parameters or keyword arguments
* when calling the function, pass in the message before or after the operation, as long as we specify which argument is which by using a comma to seperate them.
* args, there is a rule when using keyword arguments in python i.e they must come after the positional arguments
* while optional arguments are useful there is a funtional limitation to how many variables can be 
* if you want to allow users to pass in any number of variables, use the asterisk symbol before the argument name to create a pointer to the inputted variables.
* There is a rule when using keyword arguments in Python i.e. they must come after the positional arguments.
* The order of the first two arguments is important and cannot be changed. However, after these mandatory arguments, the keyword arguments can be in any order.
* While optional arguments are useful, there is a functional limitation to how many variables can be anticipated.
* If we want to allow users to pass in any number of variables, use the asterisk symbol before the argument name to create a pointer to the inputted variables.
* in order to handle keyword arguments, a method called kwargs can be used. Kwags is short for keyword arguments.
* Print kwargs to see that the keyword arguments are now stored as a dictionary instead of a tuple.
* This makes sense because keyword arguments have keys and values and can be passed in any order, so a dictionary is a more appropriate data structure for referencing them.

# Variable and Scope

* In our earlier section, *args and **kwargs were used to print out the arguments passed into a function.
* This allowed us to see a tuple and dictionary of the passed arguments. However, there's another method that allows us to access all the variables within a Python function without any asterisks. This method is called the "locals"
* However trying to reference outside it's scope will result in the error

  
* Locals()
   * Why is it named locals? These are the variable names that are only accessible locally within the function.
   * Remember, variables can be defined by any name within the function definition, and it will be available anywhere within that function.
   * However, trying to reference a variable outside its scope will result in an error.
   * in Python, there are two types of variables: local variables, which are defined inside the function, and global variables, which are defined outside the function in the main code block.
   * Thankfully, Python comes with a handy built-in function called globals that enables us to retrieve all of these variables.
 
* Global()
   * global variables are declared outside the function, you can access them throughout the program
   * if we define a vraible, meessage in the global scope and print in both functions, we can see they have access to it
   * pythom has multiple has a lot of backgrounds processes going on the scope of variables available.
 
 * lambda funcions
   * lambda functions can come in handy when you need to pass a function as an argument to another python function, such as sorted function that sorts a list of values
   * for instance if there is a list dictionaries and it needs to be sorted them based on a specific key, use the key parameter of sorted function
   * lambda functions are consise and convient for writing small functions that you need while writing code
   * use lambda function when an anonymous function is required for a short period of time
   * lambda use one expression

# Error handling and exception

* When working with Python, notice that sometimes these problems are referred to as errors, while other times are called exceptions.
* If official Python documentation is consulted, you will find that exceptions are determined during runtime and can be retried, whereas errors cannot be retried.
* there are numerous exceptions to this rule, even within the official Python code, it is not worth worrying too much about the terminology.
* in any case, they all function in a similar manner. Here is a controversial opinion: errors and exceptions are basically the same thing.
* All Python errors and exceptions ultimately stem from a class called the base exception. For instance, the division by zero error is a type of arithmetic error, which is a type of exception, which in turn extends the base exception class.
* he base exception class provides useful and powerful properties to exceptions, such as halting code execution and providing information about why and how the execution was halted.
* try/except - this is a zero division error. We have caught this exception and it will not be raised anymore. It is simply a class, it has attributes, you can create them, and they can even be returned.
* exceptions are nothing to worry about, but they do require some careful consideration.

# Catching exception by type

* We are going to catch the zero division specifically. There was a zero division error, and now that prints out. A type error statement can also be added, except type error and printed. But of course, there was a zero division error, not a type error. 

# Custom decorators

* learnt how custom decorators work and they can be created.
* got to know how they work.

# Raising Exceptions

* Add an argument and say if n is equal to zero, we raise an exception. Otherwise, we print n.
* an else statement is not used when raising an exceptions
* this is not needed because once the exception is raised, this execution will halt, and throw this exception and then the print n will never be reached.
* We, therefore, do not need an else statement there.


 </details>

 
 <details>
 <summary> Week 3 </summary>

 # GUI

 * learnt how to build a gui
 * learnt how to use Tkinter

</details>
 

