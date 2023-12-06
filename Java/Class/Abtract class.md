# abstract classes
Data abstraction is the process of hiding certain details and showing only essential information to the user.<br/>
+ Abstract class: is a restricted class that cannot be used to create objects (to access it, it must be inherited from another class).
+ Abstract method: can only be used in an abstract class, and it does not have a body.
+ The body is provided by the subclass (inherited from).<br/>
<pre>
  abstract class Animal {
  public abstract void animalSound();
  public void sleep() {
    System.out.println("Zzz");
  }
}
</pre>
use the extends keyword to inherit from a class<br/>
<pre>
  // Abstract class
abstract class Animal {
  // Abstract method (does not have a body)
  public abstract void animalSound();
  // Regular method
  public void sleep() {
    System.out.println("Zzz");
  }
}
// Subclass (inherit from Animal)
class Pig extends Animal {
  public void animalSound() {
    // The body of animalSound() is provided here
    System.out.println("The pig says: wee wee");
  }
}

class Main {
  public static void main(String[] args) {
    Pig myPig = new Pig(); // Create a Pig object
    myPig.animalSound();
    myPig.sleep();
  }
}
</pre>
# Important Points 
WhyAnd When To Use Abstract Classes and Methods?<br/>
To achieve security - hide certain details and only show the important details of an object.
