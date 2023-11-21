# Class inheritance
+ way for one class to extend another class.
<pre>
  class Animal {
  constructor(name) {
    this.speed = 0;
    this.name = name;
  }
  run(speed) {
    this.speed = speed;
    alert(`${this.name} runs with speed ${this.speed}.`);
  }
  stop() {
    this.speed = 0;
    alert(`${this.name} stands still.`);
  }
}
let animal = new Animal("My animal");
  class Rabbit extends Animal {
  hide() {
    alert(`${this.name} hides!`);
  }
}
let rabbit = new Rabbit("White Rabbit");
rabbit.run(5); // White Rabbit runs with speed 5.
rabbit.hide(); //
</pre>
**to find rabbit.run method, the engine checks (bottom-up on the picture):<br/>**
The rabbit object (has no run).<br/>
Its prototype, that is Rabbit.prototype (has hide, but not run).<br/>
Its prototype, that is (due to extends) Animal.prototype, that finally has the run method.
<pre>
Any expression is allowed after extends
Class syntax allows to specify not just a class, but any expression after extends.
For instance, a function call that generates the parent class:
</pre>
## Overriding a method
Classes provide "super" keyword for that.<br/>
+ super.method(...) to call a parent method.
+ super(...) to call a parent constructor (inside our constructor only).
<pre>
  class Animal {

  constructor(name) {
    this.speed = 0;
    this.name = name;
  }
  run(speed) {
    this.speed = speed;
    alert(`${this.name} runs with speed ${this.speed}.`);
  }
  stop() {
    this.speed = 0;
    alert(`${this.name} stands still.`);
  }
}
class Rabbit extends Animal {
  hide() {
    alert(`${this.name} hides!`);
  }
  stop() {
    super.stop(); // call parent stop
    this.hide(); // and then hide
  }
}
let rabbit = new Rabbit("White Rabbit");
rabbit.run(5); // White Rabbit runs with speed 5.
rabbit.stop(); // White Rabbit stands still. White Rabbit hides!
</pre>
## Overriding constructor
if a class extends another class and has no constructor, then the following “empty” constructor is generated:
<pre>
  class Rabbit extends Animal {
  // generated for extending classes without own constructors
  constructor(...args) {
    super(...args);
  }
</pre>
**Constructors in inheriting classes must call super(...), and (!) do it before using this.**<br/>
   When a regular function is executed with new, it creates an empty object and assigns it to this.<br/>
  But when a derived constructor runs, it doesn’t do this. It expects the parent constructor to do this job.<br/>
  <pre>
    Example:
    class Animal {
  constructor(name) {
    this.speed = 0;
    this.name = name;
  }
  // ...
}
class Rabbit extends Animal {
  constructor(name, earLength) {
    super(name);
    this.earLength = earLength;
  }
  // ...
}
// now fine
let rabbit = new Rabbit("White Rabbit", 10);
alert(rabbit.name); // White Rabbit
alert(rabbit.earLength); // 10
  </pre>
## Important Points
+ Any expression is allowed after extends.<br/>
+ Arrow functions have no super.<br/>
+ In other words, the parent constructor always uses its own field value, not the overridden one.<br/>
  
