# Welcome to Dipok's Education Hub

This hub provides a context for knowledge production and innovation through education and training.

## Express and Node JS Interview Questions

### Q1.What is Node js ?

Node Js is one of the most popular and powerful server technologies today.
It allows you built the entire website only in one programming Language i.e Javascript. Node js is free and open source server technology that uses Javascript to create complete web software.It runs on various platforms like Windows, Linux, Unix, Mac OS X, etc.

### Q2.Explain CLI.

CLI stands for Command Line Interface. It is a utility or program on your computer where users type commands to perform some action or run some script rather than clicking on the screen.
There are different types of command line interfaces depending on which operating system you are using. We have listed some of them below.

Bash on Linux.
Terminal of Mac.
Command Prompt or Powershell on Windows
Shell/ Command line/terminal on Unix and Ubuntu

### Q3.In which Language Node Js is written ?

Node js is written in C, C++,JavaScript.It uses Google’s open source V8 Javascript Engine to convert Javascript code to C++.

### Q4.Who is the author of Node Js ?

Node Js is written by Ryan Dahl.

### Q5.Explain What is a Javascript Engine ?

A Javascript Engine is a program that converts code written in Javascript to something that computer processor understands.

### Q6.Explain V8 Engine ?

V8 is Google’s open source high-performance JavaScript engine, written in C++ and used in Google Chrome, the open source browser from Google, and in Node.js, among others. It implements ECMAScript as specified in ECMA-262, and runs on Windows 7 or later, macOS 10.5+, and Linux systems that use IA-32, ARM, or MIPS processors. V8 can run standalone or can be embedded into any C++ application.
Source: https://developers.google.com/v8/

### Q7.Explain ECMAScript ?

ECMAScript is the standard on which Javascript is based on. It was created to standardize Javascript. It is commonly used for client-side scripting on the World Wide Web and used by Node Js for writing server applications and services.

### Q8.How can you check the installed version of Node Js ?

Use node -v command to check the installed version of Node Js.

### Q9.Explain What is NPM ?

NPM stands for node package manager. It is default Package Manager for JavaScript programming language. NPM is used for installing/updating packages and modules of Javascript.

### Q10.Explain Modules in Node Js ?

Modules are reusable block of code whose existence does not impact other code in any way. It is not supported by Javascript. Modules are introduced in ES6. Modules are important for Maintainability, Reusability, and Namespacing of Code.

### Q11.What are CommonJs Modules ?

CommonJS Modules is the Standard how to code modules are structured. It specifies an ecosystem for JavaScript outside on the server or for native desktop applications.

### Q12.For what require() is used in Node Js ?

require() is used to include modules from external files in Node Js. It is the easiest way to include a module in Node. Basically require is a function that takes a string parameter which contains the location of the file that you want to include. It reads the entire javascript file, executes the file, and then proceeds to return the exports object.
Syntax:

```
require('path');
```

### Q13.Explain module.exports in Node Js ?

The method or variable defined in modules cannot be directly accessible by the outer world, that means you cannot call a module member from the external file. In order to access module member, we need to export the functions or variables of modules using module.exports method.
Syntax and usage:

```node
// greet.js
var greet=function(){
console.log("hello World");
}
module.exports=greet;

//In app.js

var greet=require('./greet.js');

greet();
```
### Q14.Is Node.js Single-threaded ?

Yes, Node Js is single threaded to perform asynchronous processing. Doing async processing on a single thread could provide more performance and scalability under typical web loads than the typical thread-based implementation.

### Q15.What are events ?

An event is an action or occurrence recognized by software/app that is handled by event handler by writing a code that will be executed when the event fired.
Mouse move, Click, file copied or deleted are some examples of events.
In Node Js there are two types of events.

1)System Events: The event that comes from the C++ side.
2)Custom Events: Custom events are user-defined events.
 
### Q16.Explain event loop in Node Js ?

In Node Js processes are single threaded, to supports concurrency it uses events and callbacks. An event loop is a mechanism that allows Node.js to perform non-blocking I/O operations.
 
### Q17.How to create a simple server in Node js that returns Hello World ?

By writing following line of code, you can create a server in Node Js.

``` node
var http =require('http');
http.createServer(function(req,res){

res.writeHead(200,{'Content-Type':'text/plain'});
res.end('Hello World\n');

}).listen(1320,'127.0.0.3');
```
