oop-lesson2-quiz
================

Lesson 2 quiz


1. @a = 2
   @a is an instance variable with a Fixnum value of 2

   user = User.new
   user is a new intance of the User object

   user.name
   This is calling the getter method on the name attribute of the User object

   user.name = "Joe"
   This is setting the name attribute using the setter method of the User object

2. How does a class mixin a module?
   To mixin a module, the keyword 'include' is used at the beginning of the class:  include 'MyModule'

3. What's the difference between class variables and instance variables?
   Class variables are instantiated with the @@ and can be passed down to subclasses, where instance variables are isolated to a        specific instance with an @ and are not inheritable.

4. What does attr_accessor do?
   It's a ruby method that allows an attribute or instance variable to be called directly on the object by using built in getter and setter methods.

5. How would you describe this expression: Dog.some_method
   Dog is calling a class method.

6. In Ruby, what's the difference between subclassing and mixing in modules?
   Subclassing is done through inheritance where mixing in modules is done inside the class by using "include".  This is usually when classes have multiple inheritances or when certain behaviors are shared among classes, but not every single one of them.

7. Given that I can instantiate a user like this: User.new('Bob'), what would the initialize method look like for the User      class?
   def initialize(name)
     @name = name
   end

8. Can you call instance methods of the same class from other instance methods in that class?
   Yes.

9. When you get stuck, what's the process you use to try to trap the error?
   Debugging by using binding.pry from the pry gem.
