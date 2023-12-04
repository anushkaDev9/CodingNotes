# Encapsulation
to make sure that "sensitive" data is hidden from users. To achieve this, you must:<br/>
   + declare class variables/attributes as private<br/>
   + provide public get and set methods to access and update the value of a private variable<br/>
# Get and Set
private variables can only be accessed within the same class (an outside class has no access to it). <br/>
However, it is possible to access them if we provide public get and set methods.<br/>
The get method returns the variable value, and the set method sets the value.<br/>
<pre>
  public class Person {
  private String name; // private = restricted access
  // Getter
  public String getName() {
    return name;
  }
  // Setter
  public void setName(String newName) {
    this.name = newName;
  }
}
</pre>
**Explanation**
The get method returns the value of the variable name.
The set method takes a parameter (newName) and assigns it to the name variable. The this keyword is used to refer to the current object.
However, as the name variable is declared as private, we cannot access it from outside this class:
