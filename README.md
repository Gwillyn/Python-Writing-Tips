# Python Writing Tips
A repository to document some of my knowledge on Python.  
This is not intended to be interpreted by anybody BUT the author.  

# Python
Python is a high level, interpreted, OOP language. 

# Variables 
Variable names cannot start with a number and they can only contain alpha numeric characters or underscores. You can't use reserved keywords for variable names. In Python, snake_case is prefered. 
You cannot change a string variable after it is made, but changes made to a string variable can be assigned to a new variable. 

# Operators
the modulo operator % is be used to return the remainder of the division between 2 numbers. 7%2 is 1, because 7/2 is 3 with 1 left over. 

# Indexing
Python is 0 indexed, and you can access indiivdual string characters with an index of where it is. ```string = "Hello World"``` - to print 'r' = ```print(string[9])```, or ```print(string[-3])``` (the negative indexing indicates the end of the string). More than one argument can be used in cases like ```print()```, as long as they're separated by a comma.    
Use 4 spaces for indenting.  
You can also set a range of characters in a string with ```string[a:b:c]```, where ```a``` is the start, ```b``` is the end, and ```c``` is the step (or amount of elements to skip over. You can out negative indexes to reverse the elements.

# Syntaxes
```\n``` represents a new line.  
```len()``` will show the number of items in the string. So ```print(len(string))``` will print '11'.    
```type()``` will output the data type of the input.   
```.find()``` method will find a value in a variable. So if you want to find 'W' in a string = ```find('W')```.  
```.isalpha()``` method returns ```True``` if all of the characters in the string are letters when it is called. ```'something'.isalpha()``` will return ```True```.
```.lower()``` converts to lowercase.  
```not``` is an operator to make Truthy values return False. so ```if not thing.isalpha()``` would return ```False``` if it was true.
```pass``` can be used as placeholder for future code. It can save from errors. 
```str()``` is a function that converts a value into a string. It can also have attributes, like: ```str.maketrans({'r': '', 't': ''})```, which will make all ```r```s and ```t```s into empty strings. For this to work, however, you will need to call a translate method on the original string, like 
```  
string = "hello world"
string_translation = str.maketrans({'r': '', 't': ''})
translated_string = string.translate(string_translation)
```  
```filter()``` allows for the selection of items from an iterable, like a list, on the output of a function. ```filter(function, list)``` - the elements of ```list``` are included for the ```function``` to return.  
```float()``` takes a string/integer as an argument and returns a floating point number. 
# ```If``` Statements 
```if``` is followed by a condition and a colon. ```if x != 0:  
    print(x)```  
    ```else:``` can also follow to add an else statement.   
```elif``` checks additional conditions. It only works following the ```if```. 


# Loops
```for``` loops are written as ```for i in blank```. each line under the colon, in the body of the loop, has to be indented.  
```while``` loops runs a portion of code until the specified condition is ```True```. ```while condition:```. 

# Functions 
you can define functions like 
```
def function():
    code
```
Default values in parameters can be used to indicate a default if such parameter is not specified. So, ```function(parm=1)``` will set the ```parm``` parameter a default of 1.

# Lambda Functions
Are simple, anonymous functions. Like call-back functions in javascript for reference.   
defined by the ```lambda``` keyword. They are like: ```lambda x: expr``` - ```x``` would be the parameter for the expression of ```expr```.   
Using lambda functions with the ```map()``` function (which executes a function for each element in a collection of objects). Like: ```map(lambda x: x*4, [2, 4, 6])```.

# Errors 
A ```valueError``` is built in as an exception that is raised when the argument with the right type but inappropriate value is passed to a function. ```.index()``` is the same as ```find()``` but will throw a ```valueError```, if it is unable to find the substring.   
A TypeError cna be because you try to add a string to an integer. To fix this, convert the string variable into an integer using the built-in ```int``` function.  

# f-strings
allow for interpolation.  
Instead of writing ```'Something: ' + thing```, you cna use an f-string to write it like: ```f'Something: {thing}'.```  
The ```f``` needs to be written before the string, and the variable being interpolated is written in curly ```{}``` braces.  
# Luhn Algorithm
A formula used to validate a variety of identification numbers.    
It goes like this: 
```
    1. Right to Left - double the value of every second digit, if product is greater than 9 you sum the digits of it.  
    2. take sum of all the digits
    3. If that sum is a multiple of 10, the number is valid, else it is not.
```
# Dictionaries
This is a built-in data type, which is a collection of data in the form of key-value pairs.   
defined by curly braces ```{}```. Think of them as objects in javascript for reference.

# List Comprehensions 
A more concise way of constructing lists in Python. 

# Import
You can import Python modules to get different functionalities, like the ```random``` import. others include: ```secrets, string, ```.
