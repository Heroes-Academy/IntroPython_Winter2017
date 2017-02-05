Dictionary Exercises
====================

Dictionaries are much like lists.  They store collections.
However, you can only index into them.  This is because they are **mapping** types. 
They let you map from keys to values. 

.. code-block:: python
    :linenos:
    
    # two ways to create
    animal = {}
    animal = dict()
    
    animal['name'] = "Euclid"
    animal['age'] = 2
    animal['species'] = "Bunny"
    
Using the example above, create a dictionary for a pet or a family member. 
The "keys" can be whatever you want.  The keys I used were 'name', 'age', and 'species'.  

You can then print out the values in this dictionary!

.. code-block:: python
    :linenos:
    
    print("{} is a {} year old {}!".format(animal['name'], animal['age'], animal['species']))
    

Exercise 1
----------

Create a dictionary for a person  you know.  Have it include their name, their age, and how you know them. 
After that, print it out like I've done above. 

Exercise 2
----------

Dictionaries can be used to look things up too!  For example, you can use a dictionary
to look up a password like the following:

.. code-block:: python
    :linenos:
    
    username = input("username> ")

    users = {}
    users['euclid'] = 'secret'
    
    if username in users:
        print("Not a valid username")
    else:
        pw = users[username]
        password = input("password> ")
        if password == pw:
            print("You made it")
            
            
Make and use a dictionary like this to print out statements for users.  
It should be a simple chat bot that looks up whatever the user says
and responds with that.  

As an example (you should include a few more).

.. code-block:: python
    :linenos:
    
    responses = {}
    responses['hello'] = "hello there"
    responses['how are you'] = "I'm good, and you?"
    

Exercise 3
----------

Turn Exercise 2 into a continuous thing that uses a while loop.
In other words, in each round of the while loop, it will ask the user for input
and the look up that input inside the dictionary. 