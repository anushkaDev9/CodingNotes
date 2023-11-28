# Conditional Statement 
+ **if** -to specify a block of code to be executed, if a specified condition is true.<br/>
+ **else** - to specify a block of code to be executed, if the same condition is false.<br/>
+ **else if**- to specify a new condition to test, if the first condition is false.<br/>
+ **switch**- to specify many alternative blocks of code to be executed.<br/>
Syntax
<pre>
  if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
</pre>
Example 
<pre>
  int time = 22;
if (time < 10) {
  System.out.println("Good morning.");
} else if (time < 18) {
  System.out.println("Good day.");
} else {
  System.out.println("Good evening.");
}
// Outputs "Good evening."
</pre>
**Ternary operator**
syntax 
<pre>
  variable = (condition) ? expressionTrue :  expressionFalse;
</pre>
example
<pre>
int time = 20;
String result = (time < 18) ? "Good day." : "Good evening.";
System.out.println(result);
</pre>
# Switch 
syntax 
<pre>
  switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
</pre>
example 
<pre>
  int day = 4;
switch (day) {
  case 1:
    System.out.println("Monday");
    break;
  case 2:
    System.out.println("Tuesday");
    break;
  case 3:
    System.out.println("Wednesday");
    break;
  case 4:
    System.out.println("Thursday");
    break;
  case 5:
    System.out.println("Friday");
    break;
  case 6:
    System.out.println("Saturday");
    break;
  case 7:
    System.out.println("Sunday");
    break;
}
// Outputs "Thursday" (day 4)
</pre>
## break Keyword
+ break keyword, it breaks out of the switch block.<br/>
+ This will stop the execution of more code and case testing inside the block.<br/>
## Default keyword
+ default keyword specifies some code to run

