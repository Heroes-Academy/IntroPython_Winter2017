Week 3: Extra Challenge
=======================

Rot 13 by hand
--------------

Rot-13 is a rotation coding scheme.
Rotation coding schemes rotate the alphabet by a certain amount to get a coded letter.

Rot-13 is special because when you shift 13 spots to encode, you shift 13 spots to decode.
So, to encode OR to decode, you can shift 13 spots as long as you make sure it wraps around!

You can find out the value of a letter with the following command:

.. code-block:: python
    :linenos:

    ascii_value = ord('a')
    print(ascii_value)
    
And you can convert back with the following:

.. code-block:: python
    :linenos:

    letter_value = chr(ascii_value)
    print(letter_value)


These ascii values are numbers which represent the letters.  

Challenge:
**********

Assume all lowercase letters, "a" is the start and "z" is the end of the alphabet.

1. Use rot-13 to decode the following message.  
2. To do this, use :code:`ord` to get the number value, add 13, then use :code:`chr` to get the character again.  
3. If the number value is larger than "z", you have to make the extra "wrap around" so that it starts counting at "a". 
 
 
Hint: for the wrap around, you can use modulo to get the remainder after "z" and then add that number to the "a" ascii value. 


The message:

.. raw:: 
    
    gur fxl vf gur yvzvg
