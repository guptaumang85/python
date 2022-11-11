## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?
Ans: Because syntax of python is human readable. And it's not in form of 0, 1(bits). That's why it's called high-level programming language. 

Q2. Why is Python called a dynamically typed language?
Ans: We don't have to define type of variables and functions as we do in Java.

Q3. List some pros and cons of Python programming language?
Ans: Pros: - Easy to understand, learn and read
           - Large commmunity and pre defined libraries
           - It's an interpreted language meaning we can directly run code from source file. Not possible in case of Java
     Cons: - Python is not very fast as it is a dynamically typed language.
           - It consumes lot of memory space.

Q4. In what all domains can we use Python?
Ans: Data Science, Web development, Quantum Computing, data Engineering, Data analytics.

Q5. What are variable and how can we declare them?
Ans: If we want to assign any value that we want to use in later part of code execution, we can alot space for it memory. 
     They are declared using assignment operator where left side of assignment opeator is the name of the variable and right side is the value.

Q6. How can we take an input from the user in Python?
Ans: Using input() function.

Q7. What is the default datatype of the value that has been taken as an input using input() function?
Ans: string.

Q8. What is type casting?
Ans: To convert one form of data type in another. For example '46' is a number in form of string. If we want to perform some mathmetical operation on this string, we first need to convert it to integer using int('46') then we can perform operations.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
Ans: I don't think so. Because as input() is written once, it will get executed once, we can get input from user once. However there's is no boundation for how much we can get as input. So we can ask user to follow certain pattern and based on it we can use the string to get multiple inputs.

Q10. What are keywords?
Ans: Keywords are predefined variable/funstions in python that cannot be used in form for user defined varaibles or functions Like input, print etc.

Q11. Can we use keywords as a variable? Support your answer with reason.
Ans: No, we cannot use them as varible as they are already defined in python library.

Q12. What is indentation? What's the use of indentaion in Python?
Ans: Indentation is to make the code more readable, and elgant. Python goes the extra mile as when should code end, what comes inside loops are all based on indentation.

Q13. How can we throw some output in Python?
Ans: Using print function. print('Umang is a good data engineer.')

Q14. What are operators in Python?
Ans: These are used to perform oprations on values, and varible. Arithmatic operator to perform mathematcal operation. Others are comparison operator like '==', boolean operators.

Q15. What is difference between / and // operators?
Ans: '/' gives result as float. '//' given result as integer.

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
Ans: print('iNeuroniNeuroniNeuroniNeuron')

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
Ans: a = input('Enter number: ')
     a = int(a)
     if a%2 == 0:
       print('number is even')
     else:
       print('number is odd')

Q18. What are boolean operator?
Ans: These operator are to perform operation on boolean value. Ex. AND, OR, NOT ==> operators

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```
Ans: 1 or 0 ==> 1
     0 and 0 ==> 0
     True and False and True ==> False

Q20. What are conditional statements in Python?
Ans: These operator are decision making operator. It's like to execute one form of code if desired condition matches or to run other line of code in different scenario. 

Q21. What is use of 'if', 'elif' and 'else' keywords?
Ans: These are conditional operator. 
     'if' (condition) ==> if condition matches we execute line of code in this block.
     'elif' (condiction) ==> if above condition fails then we check for this condition and execute if it gets true.
     'else' ==> If no condition matches then we execute this line of code.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
Ans: age = int(input('Enter your age: '))
     if age < 18:
       print("I can vote")
     else:
       print("I can't vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans: for i in numbers:
       if i%2==0:
         print(i)


Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
Ans: num1 = int('Enter number 1')
     num2 = int('Enter number 2')
     num3 = int('Enter number 3') 

     if num1 > num 2 and num1> num3:
       print(num1)
     elif num2 > num3 and num2> num3:
       print(num2)
     else:
       print(num3)

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans: for i in numbers:
       if i%5==0:
         if i>150
            continue
         if i>500:
           break
         print(i)
