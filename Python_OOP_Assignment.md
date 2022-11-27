## Python OOP Assignment
Q1. What is the purpose of Python&#39;s OOP?
Ans: Purpose is to design the software in a way that it resemble real-life with classes being in real life structure and object being created using
that real life structure.

Q2. Where does an inheritance search look for an attribute?
Ans: It will first look in the class from it's being called. If it doesn't find the it go to parent class from where we are inheriting our current class.

Q3. How do you distinguish between a class object and an instance object?
Ans: When we define any class which is also called blueprint is class object. When we instantiate the class with real values is calles instance of that class.

```
class Car:
  def __init__(self, name):
    self.name = name
```
`x = Car('Mercedes')`
here `Car` is a class object and `x` is the instance object of class `Car`

Q4. What makes the first argument in a class’s method function special?
Ans: The first argument in class's method is always `self`. `self` stands for current object. 

Q5. What is the purpose of the __init__ method?
Ans: `__init__` is the method that gets automatically called whenever we create object of a class. This is can be used to assign intial values specific to that object.

Q6. What is the process for creating a class instance?
Ans: ```
class Car:
  def __init__(self, name):
    self.name = name
```
`x = Car('Mercedes')`

here, `x` is a class instance.

Q7. What is the process for creating a class?
Ans: To crete a class we use `class NameOfTheClass:` keyword. Inside this class we define attributes, and methods related to this class.

Q8. How would you define the superclasses of a class?
Ans: ```
  class ChildClassName(SuperClassName):
```

Q9. What is the relationship between classes and modules?
Ans: Moldule makes the function and variables reusable. If we want to use some predefined functions, we can define them outside of our class and use those methods inside of a class same way we would call methods defined in the class.
```
import sys

class A:
  def __init__(self):
    self.path = sys.path
   
  def getPath(self):
    return self.path

x = A()
print(x.getPath())
```
Q10. How do you make instances and classes?
Ans: ```
class Car:
  def __init__(self, name):
    self.name = name
```
`x = Car('Mercedes')`
here, `x` is instance of class `Car`

Q11. Where and how should be class attributes created?
Ans: 
```
  class Employee:
    count = 0
    def __init__(self):
      Employee.count += 1
```

here count is class attribute and is accessible to all class objects.

Q12. Where and how are instance attributes created?
Ans: 
```  
class Employee:
    count = 0

    def __init__(self, name, age):
      self.name = name
      self.age = age
    
    def increase(self):
      Employee.count += 1
```
here, `self.name`, `self.age` are instance attributes.

Q13. What does the term &quot;self&quot; in a Python class mean?
Ans: `self` represent current obejct inside the class. It is used to call on instance methods/ attributes inside the class. `self`  is also the first argument of instance methods.

Q14. How does a Python class handle operator overloading?
Ans: Operator overloading meaning changing the definition of predefined operators/methods as per our need. For example `+` in real life used to add numbers. But we can use it to concatanate two stings, list, and even objects. We redifine methods/operators in classes to overload the operator.
```
class A:
    def __init(self, a):
        self.a = a

    def __add__(self, obj):
        return self.a + obj.a
```
```
ob1 = A('umang')
ob2 = A('gupta')
ob1.__add__(ob1, ob2)
```

Q15. When do you consider allowing operator overloading of your classes?
Ans: Given in question 14.

Q16. What is the most popular form of operator overloading?
Ans: Using `+` for strings, numbers, lists.

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?
Ans: Need to understanding of classes, objects, instance variables, class variables.

Q18. Describe three applications for exception processing.
Ans: 

Q19. What happens if you don&#39;t do something extra to treat an exception?

Q20. What are your options for recovering from an exception in your script?

Q21. Describe two methods for triggering exceptions in your script.

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of
whether or not an exception exists.

Q23. What is the purpose of the try statement?

Q24. What are the two most popular try statement variations?

Q25. What is the purpose of the raise statement?

Q26. What does the assert statement do, and what other statement is it like?

Q27. What is the purpose of the with/as argument, and what other statement is it like?

Q28. What are *args, **kwargs?

Ans: `*args` is used to pass variable number of arguments to a function. This is will `args` of type tuple.
    `**kwargs` is used to pass keyworded varaible arguments. This is will `kwargs` of type dict.

Q29. How can I pass optional or keyword parameters from one function to another?
Ans: We need to paas key, and values together that we don't have to think about order of arguments.
```
  def function(arg1, arg2, arg3):
    print("arg1 = " + arg1 + "arg2 = " + arg2 + "arg3 = " + arg3)

  function(arg1 = 'umang', arg2 = 'gupta', arg3 = 'ineuron')
```

Q30. What are Lambda Functions?
Ans: lambda functions are inline function that can have multiple argument and can be used to perform operation on those argument

```
  lambda arguments : expression
```

Q31. Explain Inheritance in Python with an example?
Ans:

```
class A:
  def getName(self):
    return 'From class A'

class B:
  def getName(self):
    return 'From class B'

class C(B,A):
  pass

objC  = C()
print(objC.getName())

```
Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of class C, which version gets invoked?
Ans: From class A

Q33. Which methods/functions do we use to determine the type of instance and inheritance?
Ans: type({methodName})

Q34.Explain the use of the 'nonlocal' keyword in Python.
Ans: `nonlocal` keyword is used in nested function to use variable defined inside function but use in nested function.
```
def learnNonLocal():
  a = 10
  def nesFunc():
    nonlocal a
    a += 5
  nesFunc()
  return a
```
```
print(learnNonLocal())
```
Q35. What is the global keyword?
Ans: it is used to to define global variables that can be outside the scope in which it is defined.
```
a = 10

def change():
  global a
  a = a + 5
  print("Value of a inside a function :", a)


change()
print("Value of a outside a function :", a)
```
