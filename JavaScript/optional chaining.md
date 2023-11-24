# optional chaining
The optional chaining ?. syntax has three forms:<br/>
+ obj?.prop – returns obj.prop if obj exists, otherwise undefined.<br/>
+ obj?.[prop] – returns obj[prop] if obj exists, otherwise undefined.<br/>
+ obj.method?.() – calls obj.method() if obj.method exists, otherwise returns undefined.<br/>
As we can see, all of them are straightforward and simple to use.<br/>
The ?. checks the left part for null/undefined and allows the evaluation to proceed if it’s not so.<br/>
A chain of ?. allows to safely access nested properties.<br/>
Still, we should apply ?. carefully, only where it’s acceptable, according to our code logic, that the left part doesn’t exist.<r/>
So that it won’t hide programming errors from us, if they occur.<br/>
