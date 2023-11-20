# Constructor
+ The regular {...} syntax allows us to create one object. But often we need to create many similar objects, like multiple users or menu items and so on.<br/>
+ That can be done using constructor functions and the "new" operator.<br/>
## Constructor function
+ They are named with capital letter first.<br/>
+ They should be executed only with "new" operator.<br/>
<pre>
  function User(name) {
  this.name = name;
  this.isAdmin = false;
}
let user = new User("Jack");
alert(user.name); // Jack
alert(user.isAdmin); // false
</pre>
**function is executed with new, it does the following steps:**
1)A new empty object is created and assigned to this.<br/>
2)The function body executes. Usually it modifies this, adds new properties to it.<br/>
3)The value of this is returned.<br/>
## Constructor mode test: new.target (advance Topic)
 we can check whether it was called with new or without it, using a special new.target property.<br/>
It is undefined for regular calls and equals the function if called with new:<br/>
## Return from constructors
+ constructors do not have a return statement<br/>
If there is a return statement, then the rule is simple:<br/>
+ If return is called with an object, then the object is returned instead of this.
+ If return is called with a primitive, it’s ignored.<br/>
<pre>
  return with an object returns that object, in all other cases this is returned.
For instance, here return overrides this by returning an object:
  
</pre>
## Methods in constructor
constructor function may have parameters that define how to construct the object, and what to put in it.<br/>
Of course, we can add to this not only properties, but methods as well.<br/>
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
**Problem-Create a constructor function Calculator that creates objects with 3 methods:
read() prompts for two values and saves them as object properties with names a and b respectively.
sum() returns the sum of these properties.
mul() returns the multiplication product of these properties**
<pre>
  sol-function Calcualator(a,b){
 this.read=function(){
    this.a=a;
    this.b=b;
    console.log(`Number are ${a}+${b}`)
 }
 this.sum=()=>{
    console.log(`Sum=${a+b}`)
 }
 this.mul=()=>{
    console.log(`Mul= ${a*b}`)
 }
}
let calcualator=new Calcualator(2,3)
calcualator.read();
calcualator.sum();
calcualator.mul()
</pre>
