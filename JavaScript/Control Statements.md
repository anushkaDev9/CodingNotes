# Control Statements 
perform different actions for different decisions.<br/>
**1)if statement**- to specify a block of JavaScript code to be executed if a condition is true.<br/>
**2)else statement**- to specify a block of code to be executed if the condition is false.<br/>
**2)else if statement**- to specify a new condition if the first condition is false.<br/>
<pre>
 if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
</pre>
**3)switch statement**-to select one of many code blocks to be executed.
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
## Important Points
<pre>
 The switch expression is evaluated once.
The value of the expression is compared with the values of each case.
If there is a match, the associated block of code is executed.
If there is no match, the default code block is executed.
</pre>
