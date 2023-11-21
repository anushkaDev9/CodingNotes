## Internal and external interface
+ Internal interface – methods and properties, accessible from other methods of the class, but not from the outside.<br/>
+ External interface – methods and properties, accessible also from outside the class.
+**there are two types of object fields (properties and methods):**
+ Public: accessible from anywhere. They comprise the external interface. Until now we were only using public properties and methods.<br/>
+ Private: accessible only from inside the class. These are for the internal interface.
## Getter/setter functions

<pre>
  class CoffeeMachine {
  _waterAmount = 0;
  setWaterAmount(value) {
    if (value < 0) value = 0;
    this._waterAmount = value;
  }
  getWaterAmount() {
    return this._waterAmount;
  }
}
new CoffeeMachine().setWaterAmount(100);
</pre>
