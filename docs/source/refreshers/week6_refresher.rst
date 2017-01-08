Week 6 Refresher
================


Refresher 1
-----------

Write down the variable type for all of the "x" variables. 
If it requires a calculation, write down the answer as well. 
Verify your answers using python. 
Remember that you can use "type(x)" in the iPython shell to figure out the variable type. 

.. code-block:: python
    :linenos:

    x = int('42')
    x = '5.2'
    x = str(5.5)
    x = False or True
    x = 6 / 2
    x = (2*5) % 3
    x = 3500 // 60
    x = 3500 % 60
    x = (100 % 2 == 0 and 66 % 6 == 0)
    x = 10 != 10
    

Refresher 2
-----------

.. code-block:: python
    :linenos:
    
    response = ""
    groceries = []
    
    ### TASK: fill in the blank so that the while loop does not exit
    ### until the variable response is equal "quit"
    while _____:
    
        print("Awesome Refresher Menu.")
        print("=======================")
        print(" [1] Print grocery list")
        print(" [2] Add new grocery item")
        print(" [3] Remove a grocery item")
        print(" [4] Delete the list and start again")
        
        ### TASK: fill in the blank to tell the user what they should type 
        ### and how they can exit
        response = input("____")
        
        if response == "1":
            ### TASK: replace this with the following things:
            ###     1. An if statement that checks the length of the variable "groceries"
            ###     2. If it is larger than 0, use a for loop to print out the items
            ###     3. If it isn't, print that the grocery list is empty
            print(groceries)
        
        elif response == "2":
            new_item = input("Ok, what do you want to add? >> ")
            ### TASK: "append" the new item to the grocery list here
        
        elif response == "3":
            ## TASK: fill in the blank to ask for the item to delete
            deleting_item = input("_____")
        
            ### now we see if the item is even in the grocery list
            if deleting_item in groceries:
                ## TASK: put a success message here
                print("_____")
                ## we will delete by finding the index and deleting that
                index = groceries.index(deleting_item)
                del groceries[index]
        
        elif response == "4":
            print("Grocery list is reset!")
            ## TASK: set the variable "groceries" to equal a blank list!
            
        elif response == "exit":
            ## TASK: print out an exit message
            print("_____")
        
        else:
            ## TASK: print out an error message and show the user
            ## the response they had typed (aka, print out the response)