Week 3: If Statements
=====================


Syntax
------

.. code-block:: python
    :linenos:

    var1 = True
    var2 = False
    
    if var1:
        print("var1 is True!")
    
    if not var2:
        print("'not var2' is True!")
    
    if var2:
        print("This will never print")
    elif not var1:
        print("This won't print either!")
    else:
        print("This is the final catch-all condition!")
        
Exercises
---------
    
If-Menus
********

.. code-block:: python
    :linenos:
    
    print("This could be a menu!")
    print("\t 1. Hear a joke!")
    print("\t 2. Hear your fortune!")
    
    # var1 can be
    var1 = "1"
    # also, remember you can convert var1 to an int by:
    # var2 = int(var1)
    # or
    # var1 = int(var1)
    
    if #####fill this in######:
        print("What mood was the bunny in?  He was very hoppy!")
    elif #####fill this in######:
        print("You will have an awesome code-filled life!")
    else:
        print("You did not select a real menu option.. sad")
    

Inputs and Ifs
**************

.. code-block:: python
    :linenos:
    
    print("Welcome to my practice login screen")
    username = input("Username> ")
    password = input("Password> ")
    
    ##### Fill in the if, elif, and else to test for two usernames.
    username0 = "euclid"
    password0 = "bunny"
    
    if username0 == "euclid":
        if password0 == "bunny"
            print("You logged in!")
        else:
            print("Wrong password!")
    
    elif #### username 1 ####
        if #### password 1 ####
        
        else
    
    elif #### username 2 #####
        if  #####password 2 #####
        
        else
        
    else
        print("I don't know that username!")
        
        
        
Bonus
*****

Change the above code so that instead of having nested :code:`if` statements,
it uses a boolean :code:`and` to combine the username and password tests together. 