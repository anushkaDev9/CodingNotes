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
