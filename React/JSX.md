# JSX 
+ JSX- JavaScript XML<br/>
+ produces elements that are rendered into a DOM, in order to specify what the output must look like.<br/>
+ JSX enables the developer to create a virtual DOM using XML syntax. It compiles down to pure JavaScript (React.createElement function calls),
  therefore, it can be used inside any valid JavaScript code.<br/>
<pre>
  example:-
  var greeting = <h1>Hello React!</h1>
  var canGreet = true; 
if(canGreet) { 
   greeting = <h1>Hello React!</h1> 
}
  function Greeting() { 
   return <h1>Hello React!</h1> 
   
} 
greeting = Greeting()
  function Greet(message) { 
   ReactDOM.render(message, document.getElementById('react-app') 
} 
Greet(<h1>Hello React!</h1>)
</pre>
## Attributes in JSX
+ htmlFor instead of for <br/>
+ tabIndex instead of tabindex <br/>
+ onClick instead of onclick <br/>
**Reference https://www.tutorialspoint.com/reactjs/reactjs_jsx.htm*
