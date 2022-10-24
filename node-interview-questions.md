# Node - Interview Questions

## Questions: 

- [1] What is Node.js? Where can you use it?
- **Explain:** Node.js is an open sourse server enviornment that is free and runs on various platforms such as windows, linux, mac OSX, etc. Node.js can generate dynamic page and allows users to create, open, read, write, delete, and close files directly within the server 

- **Use:** 
- **Example:**

- [2] Why use Node.js?
- **Explain:** Use for backend development building high-scale apps that need to support multiple concurrent requests.

- **Use:** It's easy to start/use for beginners.

- **Example:**

- [3] What are the features of Node.js?
- **Explain:** it's easy to use, scalable, speed, packages

- **Use:**

- **Example:**

- [4] How do you upgrade NPM to a new version in Node.js?
- **Explain:** To update NPM, use the following command: npm install -g npm.

- **Use:**
- **Example:**

- [5] Why is Node.js Single-threaded?
- **Explain:** can handle more concurrent client's requests with ease, each thread will use the same node archetechture because the javascript is single-threaded.

- **Use:**
- **Example:**

- [6] Explain callback in Node.js.

- **Explain:** A callback is a function which is called when a task is completed.

- **Use:** this helps in preventing any kind of blocking and allows other code to run in the meantime.

- **Example:** Callback is called when task get completed and is asynchronous equivalent for a function

- [7] What is callback hell in Node.js?
- **Explain:** Callback hell in Node. js is the situation in which we have complex nested callbacks thereby making a pyramid structure that affects the readability and maintainability of the code. 

- **Use:**
- **Example:**  essentially nested callbacks stacked below one another forming a pyramid structure. Every callback depends/waits for the previous callback, thereby making a pyramid structure that affects the readability and maintainability of the code.

- [8] How do you prevent/fix callback hell?
- **Explain:** There are four solutions to callback hell:
     Write comments
    Split functions into smaller functions
    Using Promises
    Using Async/await
- **Use:**
- **Example:**

- [9] Explain the role of REPL in Node.js.
- **Explain:** A Read-Eval-Print Loop, or REPL, is a computer environment where user inputs are read and evaluated, and then the results are returned to the user

- **Use:** used for processing Node. js expressions.

- **Example:** the Node.js console, IPython, the Bash shell, and the developer console found in most web browsers.

- [10] Name the types of API functions in Node.js.
- **Explain:** You can find two types of API functions in Node.js, namely Synchronous, blocking functions, and Asynchronous, non-blocking functions.

- **Use:**
Asynchronous use: these functions allow working further while the request is being handled. Example: Emails, online forums
[4:14 PM]
Synchronous use: the application will request and wait for a response until the value is returned. Example: Instant messaging, video meetings 
- **Example:**

- [11]] What are the functionalities of NPM in Node.js?
- **Explain:** first it is an online repository for the publishing of open-source Node.js projects; second, it is a command-line utility for interacting with said repository that aids in package installation, version management, and dependency management.

- **Use:** Manage local dependencies of project's tools. Manage globally-installed project's tools.
Manage multiple versions of code and code dependencies. Download standalone tools you can use right away. NPM provides package-lock. json which displays all dependencies of the project. 

- **Example:** npm is very simple to use: you only have to run npm install async, and the specified module will be installed in the current directory under ./node_modules/. Once installed to your node_modules folder, you'll be able to use require() on them just like they were built-ins.

- [12] What is the difference between Node.js and Ajax?
- **Explain:** NodeJs is an open-source framework based on JavaScript v8 engine. AJAX is a web development technique for making asynchronous calls to the server.

- **Use:** Node.js makes it possible to run javascript outside of the browser. AJAX works on the browser or outside the browser.

- **Example:** Node is used for creating a server machine or serving static or dynamic files around the Internet. Ajax is used for fetching data from API endpoints.

- [13] What are "streams" in Node.js? Explain the different types of streams present in Node.js.
- **Explain:** Streams are objects that allows developers to read/write data to and from a source in a continuous manner. There are four main types of streams in Node. js; readable, writable, duplex and transform. Each stream is an eventEmitter instance that emits different events at several intervals

- **Use:** The readable stream is a stream that is used for read operations. The writable stream as the name suggests is a stream used for write operations. A duplex stream is a stream that performs both read and write operations. A transform stream is a stream that uses it input to compute an output.


- **Example:**

- [14] Explain chaining in Node.js.
- **Explain:** Promise chaining is a syntax that allows you to chain together multiple asynchronous tasks in a specific order

- **Use:** This is great for complex code where one asynchronous task needs to be performed after the completion of a different asynchronous task

- **Example:**

- [15] What are Globals in Node.js?
- **Explain:** Node. js global objects are global in nature and they are available in all modules. 

- **Use:** The Buffer class is an inbuilt globally accessible class that means it can be used without importing any module. The Buffer class is used to deal with binary data. Buffer class objects are used to represent binary data as a sequence of bytes. 

console: It is an inbuilt global object used to print to stdout and stderr. 

global: It is a global namespace. Defining a variable within this namespace makes it globally accessible. 

- **Example:** 

- [16] What is Event-driven programming?
- **Explain:** Event-driven programming is a paradigm where entities (objects, services, and so on) communicate indirectly by sending messages to one another through an intermediary. INO event listeners

- **Use:** Depending on the specific application, event-driven processing can improve responsiveness, throughout and flexibility.

- **Example:** Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered.

- [17] What is Event loop in Node.js? And how does it work?
- **Explain:** Event loop is an endless loop, which waits for tasks, executes them and then sleeps until it receives more tasks. 

- **Use:** The Event Loop starts at the moment Node.js begins to execute your index.js file, or any other application entry point.

- **Example:**  an example of an event loop would be creating a timer or a close event which will be repeated for as long as the application still has code that needs to be executed.

- [18] What is the purpose of module.exports in Node.js?
- **Explain:** The main purpose of module. exports is to achieve modular programming (separating the functionality of a program into independent.)

- **Use:** By Using it becomes easy to maintain and manage the code base in different modules. we can separate business logic from other modules.

- **Example:** say you want to import a module into our main file, we would call a module export so that we will be able to call our exported modules in our main file.

- [19] What is the difference between asycnhronous and non-blocking?
- **Explain:** Non-Blocking refers to the program that does not block the execution of further operations. Non-Blocking methods are executed asynchronously. Asynchronously means that the program may not necessarily execute line by line

- **Use:** Uses for non-blocking IO is to allow a single process to serve multiple requests at the same time 
 asymchronous IO is use as a form of input/output processing that permits other processing to continue before the transmission has finished

- **Example:** an example of asynchronous function is to create a callback function from within a function. 
Asynchronous, non-blocking servers - like ones made in Node - only use one thread to service all requests. This means an instance of Node makes the most out of a single thread. When requests arrive at the server, they are serviced one at a time. However, when the code serviced needs to query the DB for example, it sends the callback to a second queue and the main thread will continue running (it doesn't wait).

- [20] What is tracing in Node.js?
- **Explain:** Node. JS tracing is a module that assists in identifying and execution of the node application pattern

- **Use:**  useful for fixing memory problems, understandig what may be slowing you down, and helps node teams to have insight on performance.

- **Example:** say you want to monitor your app and location of data both on the same function and level, tracing offers a method where info generated can be traced at a central point

- [21] How will you debug an application in Node.js?
- **Explain:** Write debugger in your JavaScript code where you want debugger to stop. Now to debug, run node debug app.js. There are 7 commands you can use within the debugger(next, cont, step, out, watch, watcher, and pause)

- **Use:** uses would be to go through your code step by step to fix any hidden errors

- **Example:** say you're missing a semicolon or a right parenthesis when you run your code, debugging your code will allow you to see where your code breaks

- [22] Difference between setImmediate() vs setTimeout()?
- **Explain:** setImmediate() is designed to execute a script once the current poll phase completes. setTimeout() schedules a script to be run after a minimum threshold in ms has elapsed.

- **Use:** you would use setImmediate to execute a function right after the current event loop finishes.
setTimeout is used to call a function after the specified number of milliseconds.
- **Example:** an example of setImmediate is if you were to call the setTimeout function with zero delays an example would be using the Timers module.export.

- [23] What is process.nextTick()?
- **Explain:** process.nextTick() is used to schedule a callback function to be invoked in the next iteration of the Event Loop.

- **Use:** uses would be to clean up unanted resources, to allow users to handle errors, to try a request to run before starting the next iteration of the event loop

- **Example:** when we want one event to run after our current event finishes running so for example setting up a process.nextTick for setting up an event once a user signs in.

- [24] What is package.json? What is it used for?
- **Explain:** A package.json is a JSON file that exists at the root of a Javascript/Node project. It holds metadata relevant to the project

- **Use:** it is used for managing the project’s dependencies, scripts, version and etc.

- **Example:** The version property as it denotes the current version of the module that the package.json file is describing or The license property of a package.json file which is used to note the module that the package.json file describes. 

- [25] What is libuv?
- **Explain:** libuv is a C library originally written for Node.js to abstract non-blocking I/O operations.

- **Use:** LibUV provides support for asynchronous I/O operations. LibUV enforces an asynchronous, event-driven style of programming. 

- **Example:** to prevent wasting system resources by storing elements in a DB.

- [26] What are some of the most popular modules of Node.js?
- **Explain:** Express, AsyncJS, JSHint, Morgan, etc
- **Use:** Express.js is the fastest, unopinionated, and simplest web framework for Node.js. It was flexibly created to build simple pages, multi-pages, and hybrid apps with robust features for web and mobile development.

Asynchronous is heavily used in Node.js to ensure a non-blocking operations flow. It uses queues to monitor your workflow, allowing you to append additional tasks, attach extra callbacks, and handle errors with callbacks.

JSHint is a static analysis tool for JavaScript. It detects errors and potential problems in code.

Morgan is an HTTP request logger middleware for Node.js applications, named after Dexter. Morgan gives you insights on how your app is being used and alerts you on potential errors and issues that could be threats to your application.
- **Example:**

- [27] What is EventEmitter in Node.js?
- **Explain:** The EventEmitter is a module that facilitates communication/interaction between objects in Node
- **Use:** an emitter object basically has two main features:

       - Emitting name events.
       - Registering and unregistering listener functions.


- **Example:** Creating an event emitter instance and regiser a couple of callbacks. 

        const myEmitter = new EventEmitter();

        function c1() {
        console.log('an event occurred!');
        }

        function c2() {
        console.log('yet another event occurred!');
        }

        myEmitter.on('eventOne', c1); // Register for eventOne
        myEmitter.on('eventOne', c2); // Register for eventOne

     -When the event ‘eventOne’ is emitted, both the above callbacks should be invoked.
        
        myEmitter.emit('eventOne');