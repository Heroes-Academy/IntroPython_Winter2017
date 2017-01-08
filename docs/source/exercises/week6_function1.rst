Week 6: Functions Part 1
========================

For all of the following code, run it yourself in pycharm. 

Simplest Function
-----------------


.. code-block:: python
    :linenos:

    ### the function definition
    def hello_world():
        ### the function code block
        ### notice the indents
        print("Hello function world!")
    
    ### notice this is not indented
    ### this is how you run the function
    ### also called the function call or function execution
    hello_world()
    


Simplest Function Twice
-----------------------

Using the function above, write the code that is required to make it happen three times.



For Loop inside a Function
--------------------------

Using a :code:`for` loop and the :code:`range` function, write the following function
so that it prints the numbers up to 10

.. code-block:: python
    :linenos:
    
    def print_numbers():
        ### put the for loop here!
        
    
    print_numbers()

Calling other functions
-----------------------

Functions can even call each other.  There are several functions below. 
The first function should print out a single line. You have to fill in the blank.
It can be any message you want. 

The second function should call the other function three times.  You should not use
a loop or anything like that. 

The final function should use a for loop to call the other function. 

NOTE: the code belo will not work yet because the second two functions aren't finished!

.. code-block:: python
    :linenos:


    ### the first function
    def print_message():
        # fill in the blank
        print("___________")
        
    
    ### the second function
    def print_three():
        ## call the other function three times here
        
    ### the third function
    def print_many():
        ## call the first function inside a for loop
        
    
    ### these call the functions above    
    
    ### function 1
    print("PRINT MESSAGE FUNCTION")
    print_message()
    
    ### function 2
    print("PRINT THREE FUNCTION")
    print_three()
    
    ### function 3
    print("PRINT MANY FUNCTION")
    print_many()
    
    
    
    