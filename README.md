# Single-inheritance-python
Single inheritance is a type of inheritance where a class inherits properties and behaviors from a single parent class. This is the simplest and most common form of inheritance.

# Syntax
The syntax for single inheritance in Python is a straightforward and easy to understand. To create a new class that inheritance fro a parent class, simply specify the parent class in the class definition, inside the parentheses, like this:

    class ChildClass(ParentClass):
        # class bodoy

Example:

Let's consider a simple example of single inheritance in Python. Consider a class named "Animal" that contains the attributes and behaviors that are common to all animals.

    class Animla:
        def __init__(self, name, species):
            self.name = name
            self.species = species

        def make_sound(self):
            print("Sound made by the animal")    

If we want to create a new class for a specific type of animal, such as a dog, we can create a new class named "Dog" that inherits from the Animal class.

    class Dog(Animal):
        def __init__(self, name, bread):
            Animal.__init__(self, name, species = "Dog")
            self.bread = bread

        def make_sound(self):
            print("Bark!")    

The Dog class inherits all the attributes and behaviors of the Animal class, including the __init__ method and the make_sound method. Additionally, the Dog class has its own __init__ method that adds a new attribute for the breed of the dog, and it also override the make_sound method to specify the sound that a dog makes.

Single inheritance is a powerful tool in Python that allows you to create a new classes based on exiting classes. It allows you to reuse code, extend it to fit your needs, and make it easier to manage complex synstems. Understanding single inheritance is an important step in becoming proficient in object-orineted programming in Python.