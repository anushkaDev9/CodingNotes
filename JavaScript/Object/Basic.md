 # Objects 
 **store properties (key-value pairs) **<br/>
 + Property keys must be strings or symbols (usually strings).<br/>
 + Values can be of any type.<br/>
 <pre>
   let user = new Object(); // "object constructor" syntax
    let user = {};  // "object literal" syntax
   Example
   let user = {     // an object
  name: "John",  // by key "name" store value "John"
  age: 30        // by key "age" store value 30
};
 </pre>
 **To access a property, we can use:**<br/>
+ The dot notation: obj.property.<br/>
+ Square brackets notation obj["property"]. Square brackets allow taking the key from a variable, like obj[varWithKey]<br/>
<pre>
  alert( user.name ); // John
alert( user.age ); // 30
</pre>
**Additional operators:**
+ To delete a property: delete obj.prop.<br/>
+ To check if a property with the given key exists: "key" in obj.<br/>
+ To iterate over an object: for (let key in obj) loop.<br/>
<pre>
  let user = {
  name: "John",
  age: 30,
  isAdmin: true
};

for (let key in user) {
  // keys
  alert( key );  // name, age, isAdmin
  // values for the keys
  alert( user[key] ); // John, 30, true
}
## Additional Point.
+ intergers go in the ascending sorted order, because they are integers. So we see 1, 41, 44, 49
<pre>
  let user = {
  name: "John",
  age: 30,
  "likes birds": true  // multiword property name must be quote
};
  accessing 
  user["likes birds"] = true;
</pre>
