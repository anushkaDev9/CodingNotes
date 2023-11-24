# Object This
+ Functions that are stored in object properties are called “methods”.<br/>
+ Methods allow objects to “act” like object.doSomething().<br/>
+ Methods can reference the object as this.<br/>
<pre>
  let user = {
  name: "John",
  age: 30,
  sayHi() {
    // "this" is the "current object"
    alert(this.name);
  }
};
user.sayHi(); // John
</pre>
**this is not bound**<br/>
 + It can be used in any function, even if it’s not a method of an object.
<pre>
  let user = { name: "John" };
let admin = { name: "Admin" };
function sayHi() {
  alert( this.name );
}
// use the same function in two objects
user.f = sayHi;
admin.f = sayHi;
// these calls have different this
// "this" inside the function is the object "before the dot"
user.f(); // John  (this == user)
admin.f(); // Admin  (this == admin)
admin['f'](); // Admin (dot or square brackets access the method – doesn't matter)
</pre>
## Important Poitns 
+ Calling without an object: this == undefined<br/>
+ Arrow functions have no “this”<br/>
