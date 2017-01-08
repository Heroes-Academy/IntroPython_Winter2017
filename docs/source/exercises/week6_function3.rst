Week 6: Functions Part 3
========================

Functions can pass information out!


A basic example 
---------------

.. code-block:: python
    :linenos:
    
    def give_me_ten():
        return 10
        
    x = give_me_ten()
    print(x)
    
    
Now, write a basic example that returns your name:

.. code-block:: python
    :linenos:
    
    def your_name():
        #____
        
    name = your_name()
    ## this is the function from earlier
    greet(name)
    
    
    ### as a bonus, you can also do:
    ## greet(your_name())
    ## this is called composition
    ## it's taking the your_name output and making it the greet input


Using arguments and returns
---------------------------

.. code-block:: python
    :linenos:
    
    def center(some_string):
        centered = "{:^30}".format(some_string)
        return centered
        
    message = center("This is a nice shortcut!")
    print(message)
    
    ## BONUS: Compose the two operations above
    

Return Pig Latin
-----------------------

Fill out the following function so that it returns the pig latin version of a string!


.. code-block:: python
    :linenos:

    def piglatinify(word):
        ### save the pig latin version into a variable called new_word
        return new_word
    
    piglatinify("Heroes")
    
    ### oops, the above code doesn't save the result. how can we save it?
    ### once saved, print it!
    
    ### also, will this work?
    
    print(word)
    print(new_word)
