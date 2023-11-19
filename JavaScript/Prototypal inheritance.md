# Prototypal inheritance
+ objects have a special hidden property [[Prototype]]<br/>
+ either null or references another object<br/>
<pre>
  let animal = {
  eats: true
};
let rabbit = {
  jumps: true
};

rabbit.__proto__ = animal; // sets rabbit.[[Prototype]] = animal
</pre>
## Setter & getter 
+ prototype is only used for reading properties.<br/>
+ Accessor properties are an exception, as assignment is handled by a setter function. So writing to such a property is actually the same as calling a function.
+ <pre>
  let user = {
  name: "John",
  surname: "Smith",
  set fullName(value) {
    [this.name, this.surname] = value.split(" ");
  },
  get fullName() {
    return `${this.name} ${this.surname}`;
  }
}
let admin = {
  __proto__: user,
  isAdmin: true
};
alert(admin.fullName); // John Smith (*)
// setter triggers!
admin.fullName = "Alice Cooper"; // (**)
alert(admin.fullName); // Alice Cooper, state of admin modified
alert(user.fullName); // John Smith, state of user protected
</pre>
**No matter where the method is found: in an object or its prototype. In a method call, this is always the object before the dot.**
<pre>
Object.keys only returns own keys
for..in loops over both own and inherited keys
built-in method obj.hasOwnProperty(key): it returns true if obj has its own (not inherited) property named key
</pre>
