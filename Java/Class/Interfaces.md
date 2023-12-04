# Interfaces 
+ a completely "abstract class" that is used to group related methods with empty bodies:<br/>
<pre>
  interface Animal {
  public void animalSound(); // interface method (does not have a body)
  public void run(); // interface method (does not have a body)
}
</pre>
**To access the interface methods, the interface must be "implemented**
<pre>
  interface Animal {
  public void animalSound(); // interface method (does not have a body)
  public void sleep(); // interface method (does not have a body)
}

// Pig "implements" the Animal interface
class Pig implements Animal {
  public void animalSound() {
    // The body of animalSound() is provided here
    System.out.println("The pig says: wee wee");
  }
  public void sleep() {
    // The body of sleep() is provided here
    System.out.println("Zzz");
  }
}
class Main {
  public static void main(String[] args) {
    Pig myPig = new Pig();  // Create a Pig object
    myPig.animalSound();
    myPig.sleep();
  }
}
</pre>
# Multiple Interfaces
<pre>
  interface FirstInterface {
  public void myMethod(); // interface method
}

interface SecondInterface {
  public void myOtherMethod(); // interface method
}

class DemoClass implements FirstInterface, SecondInterface {
  public void myMethod() {
    System.out.println("Some text..");
  }
  public void myOtherMethod() {
    System.out.println("Some other text...");
  }
}
class Main {
  public static void main(String[] args) {
    DemoClass myObj = new DemoClass();
    myObj.myMethod();
    myObj.myOtherMethod();
  }
}
</pre>
# Important Points 🛑
+ Interfaces cannot be used to create objects<br/>
+ Interface methods do not have a body - the body is provided by the "implement" class<br/>
+ On implementation of an interface, you must override all of its methods<br/>
+ Interface methods are by default abstract and public<br/>
+ Interface attributes are by default public, static and final.<br/>
+ An interface cannot contain a constructor (as it cannot be used to create objects)<br/>
**Why And When To Use Interfaces**<br/>
**1) To achieve security** - hide certain details and only show the important details of an object (interface).<br/>
**2) Java does not support** "multiple inheritance" (a class can only inherit from one superclass).
  However, it can be achieved with interfaces, because the class can implement multiple interfaces. Note: To implement multiple interfaces, separate them with a comma (see example below).
