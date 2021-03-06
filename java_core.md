## Core Java - OOPs Concepts##

### Constructors 
1. #####What will be the initial value of an object reference which is defined as an instance variable?#####
The object references are all initialized to null in Java.

2. #####What is constructor?#####
Constructor is just like a method that is used to initialize the state of an object. It is invoked at the time of object creation.

3. #####Can you make a constructor final?
No, you can't

4. #####What is the purpose of default constructor?
Default constructors allow you to create objects with known, default settings and behavior. 

5. #####Why use parameterized constructor?
Parameterized constructor is used to provide different values to the distinct objects.


### static keyword
6. #####What is the static word?
 - static variable is used to refer the common property of all objects (that is not unique for each object) e.g. company name of employees,college name of students etc.
 - static variable gets memory only once in class area at the time of class loading.

7. #####What is static method?
 - A static method belongs to the class rather than object of a class.
 - A static method can be invoked without the need for creating an instance of a class.
 - static method can access static data member and can change the value of it.

8. #####Why main method is static?
because object is not required to call static method if It were non-static method,jvm creats object first then call main() method that will lead to the problem of extra memory allocation

9. #####What is difference between static (class) method and instance method?

|static or class method   |instance method|
|---|---|
|A method i.e. declared as static is known as static method.  |A method i.e. not declared as static is known as instance method.|
|Object is not required to call static method.|Object is required to call instance methods.|
|Non-static (instance) members cannot be accessed in static context (static method, static block and static nested class) directly.|static and non-static variables both can be accessed in instance methods.|
|For example: public static int cube(int n){ return n*n*n;}|For example: public void msg(){...}.|

### Inheritance
1. #####What is this in java?

It is a keyword that that refers to the current object

2. #####Why multiple inheritance is not supported in java?

To reduce the complexity and simplify the language, multiple inheritance is not supported in java.

Consider a scenario where A, B and C are three classes. The C class inherits A and B classes. If A and B classes have same method and you call it from child class object, there will be ambiguity to call method of A or B class.

Since compile time errors are better than runtime errors, java renders compile time error if you inherit 2 classes. So whether you have same method or different, there will be compile time error now.