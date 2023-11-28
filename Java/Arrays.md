# Arrays
 + store multiple values in a single variable, instead of declaring separate variables for each value<br/>
 <pre>
   type[] name={values}
 </pre>
 ## Access the Elements of an Array
 + Access an array element by referring to the index number.<br/>
<pre>
  String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
System.out.println(cars[0]);
// Outputs Volvo
</pre>
## Change an Array Element
<pre>
  String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
cars[0] = "Opel";
System.out.println(cars[0]);
// Now outputs Opel instead of Volvo
</pre>
## Array Length
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
System.out.println(cars.length);
// Outputs 4
# Multidimensional Arrays
<pre>
  int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} }
</pre>
**Access Elements** 
+ access the elements of the myNumbers array, specify two indexes: one for the array, and one for the element inside that array.<br/>
Syntax
<pre>
  int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
System.out.println(myNumbers[1][2]); // Outputs 7
</pre>
