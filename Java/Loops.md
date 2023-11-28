# Loops
execute a block of code as long as a specified condition is reached<br/>
# While loops 
loops through a block of code as long as a specified condition is true <br/>
syntax 
<pre>
  while (condition) {
  // code block to be executed
}
</pre>
example 
<pre>
  int i = 0;
while (i < 5) {
  System.out.println(i);
  i++;
}
</pre>
**Note-Do not forget to increase the variable used in the condition, otherwise the loop will never end!*
# Do/While Loop 
+ This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.<br/>
syntax
<pre>
  do {
  // code block to be executed
}
while (condition);
</pre>
example
<pre>
  int i = 0;
do {
  System.out.println(i);
  i++;
}
while (i < 5);
</pre>
# For loops
+ Statement 1 is executed (one time) before the execution of the code block.<br/>
+ Statement 2 defines the condition for executing the code block.<br/>
+ Statement 3 is executed (every time) after the code block has been executed.<br/>
syntax
<pre>
  for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
</pre>
Example 
<pre>
  for (int i = 0; i < 5; i++) {
  System.out.println(i);
}
</pre>
**For each**
syntax 
<pre>
  for (type variableName : arrayName) {
  // code block to be executed
}
</pre>
Example 
<pre>
  String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
for (String i : cars) {
  System.out.println(i);
}
</pre>
