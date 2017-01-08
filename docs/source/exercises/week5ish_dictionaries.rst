Dictionary Exercises
====================

Dictionaries are much like lists.  They store collections.
However, you can only index into them.  This is because they are **mapping** types. 
They let you map from keys to values. 

.. code-block:: python
    :linenos:
    
    # two ways to create
    euclid = {}
    euclid = dict()
    
    euclid['name'] = "Euclid"
    euclid['age'] = 2
    euclid['species'] = "Bunny"
    
Using the example above, create a dictionary for a pet or a family member. 
The "keys" can be whatever you want.  The keys I used were 'name', 'age', and 'species'.  


You can then print out the information:

.. code-block:: python
    :linenos:
    
    print("Euclid's age is {}".format(euclid['age']))
    
