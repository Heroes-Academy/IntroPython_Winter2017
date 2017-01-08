Class Exercises
===============



Class basics
------------

First class
^^^^^^^^^^^

Defining class is a recipe.  Take a look at the syntax:

.. code-block:: python
    :linenos:
    
    class Dog:
        name = 'default name'
        age = 0
        

The important part to notice is the :code:`class Dog:`.  This is what indicates the beginning of the code block.
After the class is defined, two variables are declared.  These variables are inside the class. Think of them like files in a folder. 


.. code-block:: python
    :linenos:

    class Dog:
        name = 'default name'
        age = 0

    fido = Dog()
    

This code **instantiates** the class.  This means you are using the recipe to create a new object. 

To repeat the vocabulary:

- **instantiate**: use the recipe to create an object
- **object**: a specific instance of a class. think of this like a cookie from a cookie recipe. 


Using the first class
^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python
    :linenos:

    class Dog:
        name = 'default name'
        age = 0

    fido = Dog()
    
    print("1. Fido's name: ", fido.name)
    fido.name = "Fido"
    
    print("2. Fido's name: ", fido.name)
    
    george = Dog()
    print("3. George's name: ", george.name)
    print("3. Fido's name: ", fido.name)
    
    george.name = "George"
    print("4. George's name: ", george.name)
    print("4. Fido's name: ", fido.name)
    
    
Run this example.

You will see that changing the internal properties of fido and george stay inside fido and george!
This is another example of scope. Just like inside functions are local scope, inside objects are local scope!


Getting access to internal variables
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

You can see from the last example that you access the internal variables using the dot notation. 
But, what if you wanted to write a function *inside* the object?  How can you access the variables?

Let's try this:

.. code-block:: python
    :linenos:
    
    class Dog:
        name = 'default name'
        age = 0
        
        def speak():
            print("My name is {}. Bow wow!".format(name))

    fido = Dog()
    fido.speak()
    
Do you think this will work?  Nope!  Scope doesn't let us do that!

There is a second reason why the code above won't work and that reason is also what solves things!


.. code-block:: python
    :linenos:
    
    class Dog:
        name = 'default name'
        age = 0
        
        def speak(self):
            print("My name is {}. Bow wow!".format(self.name))

    fido = Dog()
    fido.speak()


When you use the function that is inside an object, python adds a variable without you having to do anything!
That variable is called the :code:`self` variable.  


Exercises
^^^^^^^^^

- Choose an animal and write a class for it. 
- It should have at least 2 internal variables. 
- It should also have 2 functions. 


