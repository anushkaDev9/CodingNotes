# Variables 
+ contains for storing data.<br/>
**types of variables**<br/>
  + String - stores text.<br/>
  + int -stores integers (whole numbers)<br/>
  + float - stores floating point numbers.<br/>
  + char - stores single characters<br/>
  + boolean - stores values with two states<br/>
<pre>
  type variableName = value; 
</pre>
**Example**
<pre>
int myNum = 5;
float myFloatNum = 5.99f;
char myLetter = 'D';
boolean myBool = true;
String myText = "Hello";
</pre>
# Data Types 
+ **Primitive data types** - type specifies the size and type of variable values, and it has no additional method. includes byte, short, int, long, float, double, boolean and char/<br/>
+ **Non-primitive data types** - called reference types because they refer to objects,such as String, Arrays and Classes<br/>
**Difference Bwtween Primitives & non primitives
  
| Primitives    | non primitives |
| ------------- | ------------- |
| are predefined (already defined)  | created by the programmer and is not defined by Java (except for String  |
|primitive types cannot call methods to perform certain operations   |can be used to call methods to perform certain operations |
|has always a value |types can be null|
|a lowercase letter|starts with an uppercase letter.|<br/>

# Type Caasting 
+ smaller type to a larger type size<br/>
**byte -> short -> char -> int -> long -> float -> double<br/>**
+ larger type to a smaller size type<br/>
**double -> float -> long -> int -> char -> short -> byte<br/>**
+ **Widening Casting** - passing a smaller size type to a larger size type<br/>
<pre>
  int myInt = 9;
    double myDouble = myInt; // Automatic casting: int to double
</pre>
+ **Narrowing Casting**-placing the type in parentheses in front of the value.
+ <pre>
  double myDouble = 9.78d;
    int myInt = (int) myDouble; // Manual casting: double to in
</pre>
