# presentation

### hello everyone!

In my presentation, I would like to give you an overview of TypeScript

TypeScript is an open-source language which builds on JavaScript, one of the world’s most used tools, by adding static type definitions.

The goal of TypeScript is to be a static typechecker for JavaScript programs - in other words, a tool that runs before your code runs (static) and ensure that the types of the program are correct (typechecked).

Everyone loves TypeScript. It “solves” many problems JavaScript has, it is a “superset” of JavaScript, it will make your code less error-prone and pleasant to read. There are a lot of good reasons to use TypeScript.

TypeScript shares the same basic types with JavaScript:  string, number, Boolean, null, undefined, symbol, object.
but it has a couple of extra types: tuple, any, enum, void, never, array

let's look at them in more detail

### Tuple
Tuple is a data type which includes two set of values of different data types.
Imagine Tuples as organized arrays. You predefine the types in the correct order.
If we don’t follow the sorting index rules we issued for our Tuple, TypeScript will give us a hint that we didn’t follow the rules.
The Tuple expects the first value to be a number, but it’s not in this case. It’s a string "Indrek" and it is thus giving us an error.

### Any
The any type is very simple. We don’t know what type we’re dealing with, so it might as well be any.
For example:
Notice how we’re reassigning the person’s type around so many times. First, it’s a string, after a number and finally a boolean. We simply can’t be sure of the type.
A real world example would be when you’re using a third party library, and you don’t know the types.
Let’s take an array. You pull some data from an API and store it in the array. The array consists of random data. It won’t consist of only strings and numbers, nor will it have an organized structure like a Tuple. Any type can help us out here.
If you know the array only consists of one type, you can explicitly state that to the compiler, like so:

### Void
Void is used where there is no data type. For example, in return type of functions that do not return any value.
There is no meaning to assign void to a variable, as only null or undefined is assignable to void.

### Never
Never indicates the values that will never occur.
The never type is used when you are sure that something is never going to occur. For example, you write a function which will not return to its end point or always throws an exception.
In the above example, the throwError() function throws an error and keepProcessing() function is always executing and never reaches an end point because the while loop never ends. Thus, never type is used to indicate the value that will never occur or return from a function.

### Enum
Enum are a TypeScipt data type that allow the organization of number-based collections of unique identifiers.
Here’s how to define a simple enum.

### Array
An array is a special type of data type which can store multiple values of different data types sequentially using a special syntax.
TypeScript supports arrays, similar to JavaScript. There are two ways to declare an array:
1. Using square brackets. This method is similar to how you would declare arrays in JavaScript
2. Using a generic array type, Array<elementType>.
Arrays can contain elements of any data type, numbers, strings, or even objects.

Now I talk about the Benefits and Downsides TypeScript

#### Benefits:
* Catch bugs while coding instead of in production. Types allow us to recognize issues before they go wrong.
* Code completion. TypeScript is supported by most major IDE’s and text editors including VS Code and Atom. They offer powerful TypeScript integrations which complete code automatically, indicate function arguments without needing to look at the source, and provide inline error recognition.
* self-documenting code
* Improved code readability. The structure provided by TS makes it much easier to reason about new code when you have strongly typed variables, functions, and objects. It removes much of the guessing game about what shape the data will take.
* Write ES2015+. The TypeScript compiler handles all modern JavaScript and can compile backwards to previous versions of JS for compatibility.
* Optional static typing. TypeScript doesn’t require everything be statically typed, so you can incrementally convert a project.
* Great ecosystem. TypeScript has been around since 2012 and this time has allowed for it to develop a strong ecosystem. Many open source packages provide TypeScript types natively, making integration even easier.
* Increase career opportunities. TypeScript is rapidly trending upwards in adoption, and it has been integrated by many large tech companies including Google and Microsoft. By understanding TypeScript, you increase your marketability when searching for a job.

####  Downsides:
* Higher upfront cost to write new code. By requiring more code, it can slow down the development velocity of new features which may not be an ideal trade-off for every company/startup.
* Another library to stay up to date with. If you want to stay current with TS, it will require some refactoring as new versions come out.
* Learning curve for JavaScript engineers. TypeScript will take more time to ramp up engineers that have previously only been coding in JS.
* Complex types can be tricky to figure out. If you are integrating TypeScript into an existing code base, you may run into trouble getting everything typed correctly and handling complex data structures that “just worked” when it was only JS.
* More verbose code. While the structure is ultimately helpful, the trade-off is that you will be using many more characters to write the same amount of code compared to JavaScript.

Finally:
 We frequently see the question “Should I learn JavaScript, or TypeScript instead?“.
The answer is that you can’t do one without doing the other! Because TypeScript shares syntax and runtime behavior with JavaScript, anything you learn about JavaScript is helping you learn TypeScript at the same time.
Thank you for your attention!
