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

.. code-block:: python
    :linenos:
    
    class Dog:
        name = 'default name'
        age = 0
        
    def speak(some_dog):
        print("My name is {}. Bow wow!".format(some_dog.name))

    fido = Dog()
    speak(fido)
    
We can write functions which use the :code:`fido` object as its argument and 
access the internal variables!

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
That variable is called the :code:`self` variable.   This is just like having the
function outside of the :code:`class`, except that Python puts the :code:`self` variable
there automatically, so we don't have to. 


Exercises
---------

Exercise 1
^^^^^^^^^^

- Choose a new animal and write a class for it.
    - Pay attention to the pattern above. 
    - The important part is the :code:`class` keyword and the name. 
- The class should have 2 internal variables. 

You should write code that also uses your new class. For instance:

.. code-block:: python
    :linenos:

    class Dog:
        name = 'default name'
        age = 0

    pet1 = Dog()
    
    pet1.name = "Fido"
    print("First pet's name: ", pet1.name)
    

Exercise 2
^^^^^^^^^^

You should have written code that uses your class for the last exercise. 
Write a new function that takes will run this code.  It will take as input
one variable, expecting that variable to be an :code:`object` from your :code:`class`. 
It should print out all important variables in your class!

For example:

.. code-block:: python
    :linenos:

    def info(some_animal):
        print("Animal's name: ", animal.name)
    
    
Exercise 3
^^^^^^^^^^

Add an extra variable called :code:`sleep` to your class. It should start off as
:code:`False`.  Then, write two functions, called :code:`goto_sleep` and :code:`wake_up`.
The functions will take as input a single variable (like in Exercise 2).  They will
check if :code:`sleep` is :code:`True` or :code:`False`:

- in :code:`goto_sleep`, if :code:`sleep` is :code:`True`
    + nothing needs to happen
    + it should print that the animal is already asleep
- in :code:`goto_sleep`, if :code:`sleep` is :code:`False`
    + the variable :code:`sleep` should be set to :code:`True`
    + it should print that the animal is now sleeping
    
The exact same pattern happens in :code:`wake_up`, except the other way around:

- in :code:`wake_up`, if :code:`sleep` is :code:`False`
    + nothing needs to happen
    + it should print that the animal is already awake
- in :code:`wake_up`, if :code:`sleep` is :code:`True`
    + the variable :code:`sleep` should be set to :code:`False`
    + it should print that the animal is now waking up
    
    
Exercise 4
^^^^^^^^^^

Put the functions from Exercise 2 and Exercise 3 inside the class.   The code
remains exactly the same, except that the variable changes from :code:`some_animal`
will change to :code:`self` and Python will start to pass it in for us.  See the
example above again for :code:`speak` to see what I mean. 

If it were the :code:`Dog` class, your class should structurally look like:

.. code-block:: python
    :linenos:

    class Dog:

        def info(self):
            print("correct code is here!")
        
        def goto_sleep(self):
            print("correct code is here!")
        
        def wake_up(self):
            print("correct code is here!")
        
