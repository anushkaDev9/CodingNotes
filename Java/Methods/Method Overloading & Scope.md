# Method Overloading 
multiple methods can have the same name with different parameters:<br/>
<pre>
  static int plusMethod(int x, int y) {
  return x + y;
}
static double plusMethod(double x, double y) {
  return x + y;
}
public static void main(String[] args) {
  int myNum1 = plusMethod(8, 5);
  double myNum2 = plusMethod(4.3, 6.26);
  System.out.println("int: " + myNum1);
  System.out.println("double: " + myNum2);
}
</pre>
**Note-Instead of defining two methods that should do the same thing, it is better to overload one.*
# Scope
+  variables are only accessible inside the region they are created. This is called scope<br/>
**note-Variables declared directly inside a method are available anywhere in the method following the line of code in which they were declared:*<br/>
<pre>
  public class Main {
  public static void main(String[] args) {
    // Code here CANNOT use x
    int x = 100;
    // Code here can use x
    System.out.println(x);
  }
}
</pre>
# Block Scope
+ block of code refers to all of the code between curly braces {}<br/>
+ declared inside blocks of code are only accessible by the code between the curly braces, which follows the line in which the variable was declared:<br/>
<pre>
  public class Main {
  public static void main(String[] args) {

    // Code here CANNOT use x

    { // This is a block

      // Code here CANNOT use x

      int x = 100;

      // Code here CAN use x
      System.out.println(x);

    } // The block ends here

  // Code here CANNOT use x

  }
}
</pre>
