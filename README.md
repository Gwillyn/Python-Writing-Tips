# Python-Writing-Tips
A repository to document knowledge for Python.
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
# Syntaxes
```len()``` will show the number of items in the string. So ```print(len(string))``` will print '11'.    
```type()``` will output the data type of the input.   
```.find()``` method will find a value in a variable. So if you want to find 'W' in a string = ```find('W')```.  
```.lower()``` converts to lowercase.  
# ```If``` Statements 
```if``` is followed by a condition and a colon. ```if x != 0:  
    print(x)```  
    ```else:``` can also follow to add an else statement. 
# Loops
```for``` loops are written as ```for i in blank```. each line under the colon, in the body of the loop, has to be indented.  
# Functions 
you can define functions like 
```
def function():
    code
```

