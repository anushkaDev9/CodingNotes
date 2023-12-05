# Anonymous Class
a class can contain another class known as nested class. It's possible to create a nested class without giving any name.<br/>
nested class that doesn't have any name is known as an anonymous class.<br/>
must be defined inside another class. Hence, it is also known as an anonymous inner class.<br/>
**Anonymous classes usually extend subclasses or implement interfaces.*<br/>
Type can be<br/>
+ a superclass that an anonymous class extends
+ an interface that an anonymous class implements
+ <pre>
  class Polygon {
   public void display() {
      System.out.println("Inside the Polygon class");
   }
}

class AnonymousDemo {
   public void createClass() {

      // creation of anonymous class extending class Polygon
      Polygon p1 = new Polygon() {
         public void display() {
            System.out.println("Inside an anonymous class.");
         }
      };
      p1.display();
   }
}

class Main {
   public static void main(String[] args) {
       AnonymousDemo an = new AnonymousDemo();
       an.createClass();
   }
}
</pre>
**Anonymous Class Implementing an Interface**
<pre>
  interface Polygon {
   public void display();
}

class AnonymousDemo {
   public void createClass() {

      // anonymous class implementing interface
      Polygon p1 = new Polygon() {
         public void display() {
            System.out.println("Inside an anonymous class.");
         }
      };
      p1.display();
   }
}

class Main {
   public static void main(String[] args) {
      AnonymousDemo an = new AnonymousDemo();
      an.createClass();
   }
}
</pre>
**Advantages of Anonymous Classes**
objects are created whenever they are required. That is, objects are created to perform some specific tasks.
<pre>
  Object = new Example() {
   public void display() {
      System.out.println("Anonymous class overrides the method display().");
   }
};
Here, an object of the anonymous class is created dynamically when we need to override the display() method.
Anonymous classes also help us to make our code concise.
</pre>
