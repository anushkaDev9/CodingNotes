# Static properties and methods
assign a method to the class as a whole. Such methods are called static.<br/>
they are prepended by static keyword,
<pre>
  class User {
  static staticMethod() {
    alert(this === User);
  }
}
User.staticMethod(); // true
explanation 
  class User { }
User.staticMethod = function() {
  alert(this === User);
};
User.staticMethod(); // true
</pre>
## Contructor 
<pre>
  class Article {
  constructor(title, date) {
    this.title = title;
    this.date = date;
  }
  static compare(articleA, articleB) {
    return articleA.date - articleB.date;
  }
}
// usage
let articles = [
  new Article("HTML", new Date(2019, 1, 1)),
  new Article("CSS", new Date(2019, 0, 1)),
  new Article("JavaScript", new Date(2019, 11, 1))
];
articles.sort(Article.compare);
alert( articles[0].title );
</pre>
## Static properties
they look like regular class properties, but prepended by static.
<pre>
  class Article {
  static publisher = "Ilya Kantor";
}
alert( Article.publisher );
</pre>
## Inheritance of static properties and methods.
Static properties and methods are inherited.
<pre>
  class Animal {
  static planet = "Earth";
  constructor(name, speed) {
    this.speed = speed;
    this.name = name;
  }
  run(speed = 0) {
    this.speed += speed;
    alert(`${this.name} runs with speed ${this.speed}.`);
  }
  static compare(animalA, animalB) {
    return animalA.speed - animalB.speed;
  }
}
// Inherit from Animal
class Rabbit extends Animal {
  hide() {
    alert(`${this.name} hides!`);
  }
}
let rabbits = [
  new Rabbit("White Rabbit", 10),
  new Rabbit("Black Rabbit", 5)
];
rabbits.sort(Rabbit.compare);
rabbits[0].run(); // Black Rabbit runs with speed 5.
alert(Rabbit.planet); // Earth
</pre>
explanation<br/>
Rabbit extends Animal creates two [[Prototype]] references:<br/>
Rabbit function prototypally inherits from Animal function.<br/>
Rabbit.prototype prototypally inherits from Animal.prototype.<br/>
## D
## Important Points
+ Static methods aren’t available for individual objects.<br/>
+ Static  methods cannot be accessed through instantiated objects but could be accessed through the class name
