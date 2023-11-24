# Function :computer:
**Defination** - block of code designed to perform a particular task.
<pre> function name(){
  alert("welcome")
  }
name() - calls the function
</pre>
## Function Parameters and Argument
* Function parameters are the names listed in the function definition.<br/>
* Function arguments are the real values passed <br/>
<pre>function functionName(parameter1, parameter2, parameter3) {
  // code to be executed
}</pre>
## Named Function Expression
term for Function Expressions that have a name.
<pre>
  let sayHi = function func(who) {
  if (who) {
    alert(`Hello, ${who}`);
  } else {
    func("Guest"); // use func to re-call itself
  }
};
sayHi(); // Hello, Guest
// But this won't work:
func(); // Error, func is not defined (not visible outside of the function)
};
</pre>
**There are two special things about the name func, that are the reasons for it:**<br/>
 1) It allows the function to reference itself internally.<br/>
2) It is not visible outside of the function.<br/>
## CallBack Function 
Function passed as parameters.
<pre>
  function ask(question, yes, no) {
  if (confirm(question)) yes()
  else no();
}
function showOk() {
  alert( "You agreed." );
}
function showCancel() {
  alert( "You canceled the execution." );
}
// usage: functions showOk, showCancel are passed as arguments to ask
ask("Do you agree?", showOk, showCancel);
</pre>
## Important topics 🛑
* The return statement stops the execution of a function and returns a value. <br/>
* a function’s name is accessible as the “name” property.<br/>
* contextual name- if the function does not provide one, then in an assignment it is figured out from the context.<br/>
* length” that returns the number of function parameters.<br/>
* counter property to track the total calls count<br/>


