# JSX 
+ JSX- JavaScript XML<br/>
+ produces elements that are rendered into a DOM, in order to specify what the output must look like.<br/>
+ JSX enables the developer to create a virtual DOM using XML syntax. It compiles down to pure JavaScript (React.createElement function calls),
  therefore, it can be used inside any valid JavaScript code.<br/>
<pre>
  example:-
  var greeting = <p>Hello React!</p>
  var canGreet = true; 
if(canGreet) { 
   greeting = <p>Hello React!</p> 
}
  function Greeting() { 
   return <p>Hello React!<p> 
   
} 
greeting = Greeting()
  function Greet(message) { 
   ReactDOM.render(message, document.getElementById('react-app') 
} 
Greet(<p>Hello React!</p>)
</pre>
## Attributes in JSX
+ htmlFor instead of for <br/>
+ tabIndex instead of tabindex <br/>
+ onClick instead of onclick <br/>
**Reference https://www.tutorialspoint.com/reactjs/reactjs_jsx.htm*
