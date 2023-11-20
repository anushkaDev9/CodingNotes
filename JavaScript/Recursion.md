# Recursion 
+ programming pattern that is useful in situations when a task can be naturally split into several tasks of the same kind, but simpler.<br/>
+ function solves a task, in the process it can call many other functions. A partial case of this is when a function calls itself.<br/>
<pre>
  function pow(x, n) {
  return (n == 1) ? x : (x * pow(x, n - 1));
}
</pre>
**Information about the process of execution of a running function is stored in its execution context.*<br/>
**Internal data structure that contains details about the execution of a function: where the control flow is now, the current variables, the value of this (we don’t use it here) and few other internal details.*
## Recursive structures
A recursive (recursively-defined) data structure is a structure that replicates itself in parts.
Example 
**question :- The factorial of a natural number is a number multiplied by "number minus one", then by "number minus two", and so on till 1. The factorial of n is denoted as n!**<br/>
1! = 1 <br/>
2! = 2 * 1 = 2<br/>
3! = 3 * 2 * 1 = 6<br/>
4! = 4 * 3 * 2 * 1 = 24<br/>
5! = 5 * 4 * 3 * 2 * 1 = 12 <br/>
soltuion 
<pre>
  let rec=(n)=>{
    let sum=0
    n===1 ? sum=1:sum=n*rec(n-1)
    return sum
}
console.log(rec(5))
</pre>
