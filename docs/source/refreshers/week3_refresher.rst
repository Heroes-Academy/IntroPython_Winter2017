Week 3 Refresher
================

Let's refresh your memory!

Part 1: Variables and Types
---------------------------

Information
***********

There are four basic variable types

.. code-block:: python
    :linenos:

    x = 5     # int
    x = 5.0   # float
    x = "5"   # str
    x = True  # bool

Practice time
*************

For each item, write down on a sheet of paper the exact code, the result, and the type. 
As an example, I've written the first one on the white board. 

.. code-block:: python
    :linenos:

    item1 = str(5.0)
    item2 = "a" + "bunny"
    item3 = 2*2
    item4 = item2[1]
    item5 = item2[:5]
    item6 = item4 + item5
    item7 = float(item1) * 3
    item8 = int(item7)
    item9 = item8 % 2
    item10 = str(item9)
    
.. 
    item1="5.0"; str
    item2="abunny"; str
    item3=4; int
    item4="n"; str
    item5="abunn": str
    item6="nabunn"
    item7=15.0
    item8=15
    item9=1
    item10="1"


Part 2: String Practice
-----------------------

Information
***********

.. code-block:: python
    :linenos:
    
    #       012345678
    name = "Bunnyface"
    #       012345678
    # these are all negative: (but there's not enough room for the "-" for all numbers
    #      -987654321
    
    # Indexing retrieves the letter at that spot!
    name[0] #  is "B"
    name[5] # is "f"
    name[-1] # is "e"
    
    # Slicing gets the range of letters 
    # It starts with the first number
    # and it goes UP TO the second number
    name[0:4]  # is "Bunn"
    
    # Sometimes you have to use a number beyond the end of the string
    
    name[5:9]  # is "face"
    
    # you can use variables
    index = 2
    start = 4
    stop = 7
    name[index] # is "n"
    name[start:stop] # is "yfa"
    
    # you can also leave out the start of the stop, it assumes the beginning or end
    name[:stop] # is "Bunnyfa"
    name[start:] # is "yface"
    
Practice
********

For each of the following, write down the result! 

.. code-block:: python
    :linenos:

    #           01234567
    original = "Penguins"
    #           01234567
    
    item1 = original[0]
    item2 = original[4]
    item3 = original[1:5]
    item4 = item2 + item3
    item5 = item3*2 + item1
    item6 = original[-3]
    item7 = original[:-1]
    
    ### what does i need to be to make item8 equal "g"?
    # i = ?
    item8 = original[i]
    
    