Classes
=======

:code:`self`
^^^^^^^^^^^^

Self is python's way of solving the scope problem!  You can access properties of an object from outside the object using dot notation on the variable. 
While inside a function inside the object, python provides you with a variable that lets you access the rest of the object.

This is accessing the propers from OUTSIDE:

.. code-block:: python
  
    class Dog:
        name = 'default name'
        age = 0

    fido = Dog()
    
    print("1. Fido's name: ", fido.name)
    fido.name = "Fido"
    
    print("2. Fido's name: ", fido.name)
    
    
    class Dog:
        name = 'default name'
        age = 0
        
        def speak(self):
          print("This is inside! My Name: {}".format(self.name))

    fido = Dog()
    
    fido.speak()
    print("This is outside! Fido's name: ", fido.name)
    
    fido.name = "Fido"
    
    fido.speak()
    print("This is outside! Fido's name: ", fido.name)
    
    

:code:`def __init__(self)`
^^^^^^^^^^^^^^^^^^^^^^^^^^

The :code:`__init__` function is one of Python's special functions - this is indicated by the double underscore (__) on either side of the function name. :code:`init` is a keyword (like :code:`print` or :code:`if``) and Python already knows what it's used for.

When you write your own class, sometimes it's helpful to have a kind of setup function that runs whenever you make a new copy of the class. For example, if you write the :code:`Door` class we've been using as an example, you might want the :code:`Door` to print out "Hello!" the first time someone makes it. And, every new :code:`Door` that gets made will also say "Hello!"

This is what the :code:`__init__` function is for: it's a special function that runs once every time an object of that type (in our example, :code:`Door`) is made.

So, for example:
::
  class Door:
    def __init__(self):
      print("Hello!")
      
  first_door = Door()
  second_door = Door()
  
The code above will print out "Hello!" twice - once for :code:`first_door`, and again for :code:`second_door`.

That's an example of an :code:`__init__` function that doesn't take any arguments. Usually, this isn't the case - because :code:`__init__` is a setup function, you want the user to provide certain information about the object when they make it. 

Here's an example:
::
  class Door:
    def __init__(self, in_name, in_height):
      self.name = in_name
      self.height = in_height
      print("Hello! My name is " + self.name)
    
  first_door = Door("Gerald", 10)
  second_door = Door("Geraldina", 12)

In this code, when a :code:`Door` object is created, it takes two arguments: the name, and the height. These arguments are then used for setting up the Door object (i.e., they set up the properties :code:`self.name` and :code:`self.height`)
