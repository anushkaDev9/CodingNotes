# Method
+ must be declared within a class.<br/>
+ name of the method, followed by parentheses ()<br/>
+ Java provides some pre-defined methods, such as System.out.println()<br/>
<pre>
  public class Main {
  static void myMethod() {
    // code to be executed
  }
}
</pre>
<pre>
  Explanation
  myMethod() is the name of the method<br/>
  static means that the method belongs to the Main class and not an object of the Main class.<br/>
void means that this method does not have a return value. <br/>
</pre>
# Call a Method
+ myMethod() is used to print a text (the action), when it is called<br/>
<pre>
  public class Main {
  static void myMethod() {
    System.out.println("I just got executed!");
  }

  public static void main(String[] args) {
    myMethod();
  }
}

</pre>
