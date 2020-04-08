## Call Stack :
**A call stack** is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions.

- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.

- The **call stack** is primarily used for function invocation (call). Since the **call stack** is single, function(s) execution, is done, one at a time, from top to bottom. It means the **call stack** is synchronous.
 -The understanding of the **call stack** is vital to Asynchronous programming.
 a **call stack** is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call), it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.


 ### Manage function invocation (call):
   The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.

### What causes a stack overflow?
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser  has a maximum stack call that it can accomodate before throwing a stack error.
in other word If the stack takes up more space than it had assigned to it, it results in a **"stack overflow"** error.

### JavaScript error messages && debugging:

- **Reference errors**
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

- **Syntax errors**
this occurs when you have something that cannot be parsed in terms of syntax.

- **Range errors**
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

- **Type errors**
this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible.

- **Handling errors**
that shows up like that when we do not handle errors properly, meaning that anything after that error will not be executed. 

## Debugging:
- To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check.
- You can also add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values.

###  Tools to avoid runtime errors:
- **quokka** to evaluate your code as you type
- **eslint** to make sure your style guide is consistency and it will grab you an error or two along the way and
- For those of you looking to make JS a more strong typed experience you can check out stuff like TypeScript 


