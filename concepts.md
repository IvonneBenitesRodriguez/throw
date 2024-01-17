**throw** <br/>
It is a mechanism for dealing with exceptional conditions,<br/>
making code more robust, and giving a way to handle with <br/>
unexpected situations in a controlled manner.<br/>

The following are the situations where we can use **throw**<br/>

a) **To explicity signal that something unexpected or erroneous has**<br/>
happened to your code.<br/>

Example:<br/>

function divide(a,b) {<br/>
if (b === 0) {
    throw new **Error**("Cannot divide by zero!");<br/>
}
return a/b;<br/>
}<br/>

2 **Error Handling:**<br/>
By throwing an error, you can handle exceptional cases in your code<br/>
using **try...catch** blocks.<br/>
This allows to manage errors and give meaninful error messages.

try{<br/>
let result = divide(10,2);<br/>
console.log("Result:", result);<br/>

let errorResult = divide(5,0);<br/> <!--this will throw an error !>
}catch (error) {<br/>
console.error("Error:", error.message);
}