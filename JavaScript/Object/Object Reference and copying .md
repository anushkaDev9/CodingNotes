# Object references and copying

| Object | Primitives |
| ------------- | ------------- |
| stored and copyed by reference  | copied as whole  |
<pre>
  let user = { name: "John" };
let admin = user; // copy the reference
</pre>
**Comparison by reference**<br/>
+ Two objects are equal only if they are the same object.<br/>
<pre>
  let a = {};
let b = a; // copy the reference
alert( a == b ); // true, both variables reference the same object
alert( a === b ); // true
</pre>
**Cloning and merging, Object.assign**<br/>
+ copying an object variable creates one more reference to the same object<br/>
<pre>
  let user = {
  name: "John",
  age: 30
};
let clone = {}; // the new empty object
// let's copy all user properties into it
for (let key in user) {
  clone[key] = user[key];
}
</pre>
**Object.assign*<br/>
+ Object.assign(dest, ...sources)<br/>
    + The first argument dest is a target object(the one you want to duplicate).<br/>
    + Further arguments is a list of source objects.<br/>
<pre>
  let user = { name: "John" };
let permissions1 = { canView: true };
let permissions2 = { canEdit: true };
// copies all properties from permissions1 and permissions2 into user
Object.assign(user, permissions1, permissions2);
  or
let user = { name: "John" };
Object.assign(user, { name: "Pete" });
alert(user.name); // now user = { name: "Pete" }
</pre>
**Nested cloning**
properties can be references to other objects.
<pre>
  let user = {
  name: "John",
  sizes: {
    height: 182,
    width: 50
  }
};
let clone = Object.assign({}, user);
alert( user.sizes === clone.sizes ); // true, same object
// user and clone share sizes
user.sizes.width = 60;    // change a property from one place
alert(clone.sizes.width); // 60, get the result from the other one
</pre>
**For the above error use structuredClone**
+ structuredClone(object) clones the object with all nested properties.
<pre>
  let user = {
  name: "John",
  sizes: {
    height: 182,
    width: 50
  }
};
let clone = structuredClone(user);
alert( user.sizes === clone.sizes ); // false, different objects
// user and clone are totally unrelated now
user.sizes.width = 60;    // change a property from one place
alert(clone.sizes.width); // 50, not related
  or
let user = {};
// let's create a circular reference:
// user.me references the user itself
user.me = user;
let clone = structuredClone(user);
alert(clone.me === clone); // true
</pre>
**Note-Function properties aren’t supported.*<br/>
**Important Points**
1)A variable assigned to an object stores not the object itself, but its “address in memory” – in other words “a reference” to it.<br/>
2)When an object variable is copied, the reference is copied, but the object itself is not duplicated.
3)Const objects can be modified<br/>
4)structuredClone method can clone most data types, such as objects, arrays, primitive values.
5) It also supports circular references, when an object property references the object itself
