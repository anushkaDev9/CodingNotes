# Loops
## While Loop 
loops through a block of code as long as a specified condition is true.
<pre>
  while (condition) {
  // code block to be executed
}
</pre>
## Do while 
will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.
<pre>
  do {
  // code block to be executed
}
while (condition);
</pre>
### Difference between do while and while

| While       | Do while        | 
| ------------- |:-------------:| 
| Loop body is executed after the given condition is evaluated.    |Loop body is executed, and then the given condition is checked. | 
| Variables are initialized before the execution of the loop.    | Variables may initialize before or within the loop.  |  
| Entry Control Loop| Exit Control Loop.   |    
## For loop
+ for - loops through a block of code a number of times
  <pre>
  FOR LOOP
  for (set the intial point; condition;increase or decrease) {
  // code block to be executed
}
</pre>
+ for/in - loops through the properties of an object
  <pre>
    for (key in object) {
  // code block to be executed
}
Each iteration returns a key (x)
The key is used to access the value of the key
  </pre>
+ for/of - loops through the values of an iterable object
  <pre>
    for (variable of iterable) {
  // code block to be executed
}
  </pre>

+ forEach() method calls a function (a callback function) once for each array element.
  <pre>
    numbers.forEach(myFunction);
function myFunction(value, index, array) {
  txt += value;
}
  </pre>
