# Contructor operator "new" 
+ allows us to create one object<br/>
+ to implement reusable object creation code.<br/>
Example
<pre>
  function User(name) {
  this.name = name;
  this.isAdmin = false;
}
let user = new User("Jack");
alert(user.name); // Jack
alert(user.isAdmin); // false

Explanation
When a function is executed with new, it does the following steps:
A new empty object is created and assigned to this.
The function body executes. Usually it modifies this, adds new properties to it.
The value of this is returned.
</pre>
## new.target
check whether it was called with new or without it, using a special new.target property.<br/>
<pre>
  function User() {
  alert(new.target);
}
// without "new":
User(); // undefined
// with "new":
new User();
</pre>
## Return from constructors
if there is a return statement, then the rule is simple:<br/>
  + If return is called with an object, then the object is returned instead of this.<br/>
  + If return is called with a primitive, it’s ignored.<br/>
## Methods in constructor 
<pre>
  function User(name) {
  this.name = name;
  this.sayHi = function() {
    alert( "My name is: " + this.name );
  };
}
let john = new User("John");
john.sayHi(); // My name is: John
/*
john = {
   name: "John",
   sayHi: function() { ... }
}
*/
</pre>
