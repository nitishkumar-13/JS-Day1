#Task 1

1) Write a blog on Difference between HTTP1.1 vs HTTP2

HTTP1.1:

-> It works on the textual format.
-> There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.
-> It uses requests resource Inlining for use getting multiple pages.
-> It compresses data by itself.

HTTP2:

-> It works on the binary protocol.
-> It allows multiplexing so one TCP connection is required for multiple requests.
-> It uses PUSH frame by server that collects all multiple pages.
-> It uses HPACK for data compression.

2) Write a blog about objects and its internal representation in Javascript

-> It objects in JavaScript may be defined as an unordered collection of related data, of primitive or reference types, 
   in the form of “key: value” pairs. 
-> These keys can be variables or functions and are called properties and methods, respectively, in the context of an object.

-> Example of an object in JavaScript
let person = {
    name: "Nitish",
    age: 22,
    email: "abcn@example.com",
    greet: function() {
        console.log("Hello, my name is " + this.name);
    }
};

-> Internal Representation:
{
    name: "Nitishkumar S"          --> Property Name: "name", Value: "Nitishkumar S"
    age: 22                        --> Property Name: "age", Value: 22
    email: "abc@example.com"       --> Property Name: "email", Value: "abc@example.com"
    greet: <function>              --> Property Name: "greet", Value: Reference to the function
}