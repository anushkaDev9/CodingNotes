# Summary On class Inheritance 
1) To extend a class: class Child extends Parent:<br/>
    + That means Child.prototype.__proto__ will be Parent.prototype, so methods are inherited.<br/>
2) When overriding a constructor:<br/>
    + We must call parent constructor as super() in Child constructor before using this.<br/>
3)When overriding another method:<br/>
    + We can use super.method() in a Child method to call Parent method.<br/>
4)Internals:<br/>
  + Methods remember their class/object in the internal [[HomeObject]] property. That’s how super resolves parent methods.
  + So it’s not safe to copy a method with super from one object to another.
