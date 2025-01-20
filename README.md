# NamasteNode-JS-EP-03
## Episode-02 | Writing Code
----------------------------------------------------------------

**Verify installed correctly or node by writing command on Terminal**
- *node -v*
- The command node *node -v* is used to check the installed version of Node.js. If Node.js is not installed, this command will produce an error indicating that the *node* command is not installed or recognized or not found.
- *npm -v*  
- This command displays the version of **NPM** that is currently installed on your machine. 

**Writing Code In Terminal**
- **Node REPL [Read, Evaluate, Print, Loop]**
- write command on terminal *node* and then we can write and execute code on REPL.
- NodeJS is a *JS runtime environment*, and behind the scenes, it is using the *V8 engine*.
- its similar to a browser console.
- But we cannot write code in terminal for long time.
  
**Writing Code In VS Code** 
- *Create a folder on desktop.*
- *Open the Folder in VS Code.*
- *Create a file named **app.js***
- ` let name = "Node JS 03;"
    let a = 5;
    let b = 10;
    let c = a + b;
    console.log(name);
    console.log(c); `
- *open terminal using the shortcut **Ctrl + `***
- *now write command **node app.js** to run the code*

**Global Objects in NodeJs**
- In each JavaScript environment, there is always a global object defined. 
- The **global object's interface** depends on the *execution context* in which the *script* is running.
- In a *web browser*, **the global object** for most JavaScript code is **Window**, unless the script is explicitly run as a background task.
- Scripts running under *Node.js* have an object called **global** as their *global object.*

- The *window* object is a global object provided by the *browser*, not by the **V8 engine**
- In node.js, the global object is known as global, which is equivalent to the window object in the browser.
- This global object is not a part of V8 engine, it is a feature provided by Node.js 
- The V8 engine does not understands the Global, it only understands it because the node.js gives it access inside V8 engine.
- The global object offers various functionalities, such as *setTimeout()*, *setInterval()*, and many more.

# Important Note:
----------------------------------------------------------------

- When i used *console.log(this)*; at the global level in Node.js, it will *log* an **empty object,** 
indicating that *this* does not refer to the global object in this context.

**Global this**
- *Global this* is always a global object, regardless of where it is accessed,
- It was introduced in ECMAScript 2020 to provide a standardized way to refer to the global object in any envs (browesers, Node.js, etc).
- In browsers, *global* = *window*.
- In Node.js, *GlobalThis* = *global*.
  