Week 6: Functions Part 2
========================

The most important information about arguments:

1. Functions have a local context only!
2. Sending information into a function is through arguments
3. Giving a variable to a function can be described as "passing the variable in"



Functions with one arguments
----------------------------

.. code-block:: python
    :linenos:

    # finish this code by replacing the underlined parts!
    def print_this(___):
        print(____)
        
    print_this("Hello!")


Functions with more than one argument
-------------------------------------

To accept more than one argument, we simply list the variables an use commas!

.. code-block:: python
    :linenos:
    
    # finish this code by replacing the underline parts!
    
    def print_more(__, ____)
        ## print both of the variables separately
        
    print_more("Hello World",  "It is a great day!")
    
.. code-block:: python
    :linenos:


    def do_math(___, ____):
        ## write code here that adds the two variables
        ## then it prints the result
        
    
    do_math(10, 20)



Practicing arguments more
-------------------------

Finish writing each of the following functions. You should do them one at a time
and make sure each one works before writing the next. 

.. code-block:: python
    :linenos:
    
    def print_n(message, n):
        # finish this part of the code
        # it should print the message n times
        # hint: use a for loop
        #  ____________
        
        
    print_n("Functions make life easier!", 5)
        
    def greet(name):
        ## greet the person!
        
    
    greet("Dr. Euclid Von Rabbitstein")
        
    def compute_fizzbuzz(n):
        ## write the if statement for fizz buzz!
        ## remember: if n is a multiple of 3, print "fizz"
        ##           if n is a multile of 5, print "buzz"
        ##           if n is a multiple of both 3 and 5, print "fizzbuzz"
        ##           if none of the above, print the number
        
    compute_fizzbuzz(3)
    compute_fizzbuzz(5)
    compute_fizzbuzz(15)
    
        
    def fizzbuzz_loop(n):
        ## write a for loop which goes around "n" times
        ## each time inside the for loop, call the compute_fizzbuzz(__) function
        
    fizzbuzz_loop(100)
        

Keyword arguments
-----------------

You can set default values for arguments.  
They still act as normal arguments, if you pass in the variables in, it will accept them in order.
The difference is that you can choose not to specify some variables.

**IMPORTANT**: all keyword arguments come after normal arguments. 

.. code-block:: python
    :linenos:
    
    def print_n(message, n=10):
        ### use the same for loop you had above to print the message n times
        
    print_n("[1] Functions are awesome!")
    print_n("[2] Functions are awesome!", 3)
    ### notice how i specifically specify the n in this next one
    print_n("[3] Functions are awesome!", n=3)

For this next one, I have left out all parts of the argument specification. 
You have to write it.  I have written the code.  There are two needed variables:
:code:`stop_number` and :code:`multiple_number`.  They should both have default values.
        
.. code-block:: python
    :linenos:
    
    def detect_multiples(____):
        for i in range(stop_number):
            if i % multiple_number == 0:
                print("{} is a multiple of {}".format(i, multiple_number))
    
    print("\n --Test 1-- \n")
    detect_multiples(100, 7)
    
    print("\n --Test 2-- \n")
    detect_multiples(stop_number=100, multiple_number=13)
    
    print("\n --Test 3-- \n")
    detect_multiples(multiple_number=9)
    
    print("\n --Test 4-- \n")
    detect_multiples(stop_number=20)

