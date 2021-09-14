# *FUNCTIONAL PROGRAMMING*

## *What Is Functional Programming?*
Functional programming is a programming paradigm designed to handle pure mathematical functions. This paradigm is totally focused on writing more compounded and pure functions.

JavaScript is a multi-paradigm language, which means that we can easily mix a lot of different paradigms inside a simple piece of JavaScript code. We can use object-oriented, procedural and functional programming paradigms all at the same time in JavaScript. The fact that JavaScript is multi-paradigm and allows us to work with a lot of different ways of programming is what makes this language so beautiful and powerful.

Functional programming has a few important concepts that we need to know and understand. By implementing these concepts in your applications, you will end up with more functional code. This will make a huge difference in your application, making it more readable, usable, manageable, easy to test and bug-free.

Let’s cover the important concepts about functional programming and how we can apply them in JavaScript
*  ### First-Class Objects
 What’s good about Functional Programming is its functions are first-class citizens: you can always insert functions inside a function without any restrictions present.
```
onst sum = (a, b) => a + b;

const resultSum = sum(1, 2);

const sumAgain = (a, b, sum) => sum(a, b);
```

* ### Pure Functions
One of the most important concepts in the functional programming paradigm is pure functions. Functional programming requires us to write pure and deterministic functions, and this is what makes functional programming so beautiful and useful: it forces us to write better code with pure functions, making our code easier to test and manage.
 ```
 const myName = (name) => `Hello ${name}`;

myName("Leonardo") // Should always return "Hello Leonardo"
 ```
* ### Higher-Order Functions
 A higher-order function is a function that gets a function as an argument. It may or may not return a function as its resulting output.
```
const names = ["Leonardo", "Lucas", "Bianca", "José", "Maria", "Joe"];

const sayHiToNames = names.map(name => `Hello ${name}`);
```
* ### Composition
Functional Programming won’t be completely functional without this feature. Function Composition is an act of composing/creating functions that allow you to further simplify and compress your functions by taking functions as an argument and return an output. It may also return another function as its output other than numerical/string values.
```
const splitName = (name) => name.split('_').join(' ');

const returnNameCapitalized = (name) => name.toUpperCase();

console.log(returnNameCapitalized(splitName('leonardo_maldonado')));
```
* ### Declarative vs. Imperative
 Declarative and imperative programming are different programming paradigms that can help you to achieve different results.

Declarative programming is a programming paradigm where we specify the program logic without describing the flow control. Declarative programming is all about what to do to achieve a certain result.
```
const numbers = [1, 2, 3, 4, 5];

const sumNumbers = (n) => n.reduce((acc, current) => acc + current);
```
* ### Immutability
 very important concept in functional programming is immutability. An immutable object is an object that can’t be modified after its creation. Imagine that we have an object and we want to modify this object by adding a new element—what should we do? We should create a new object, a copy of the actual object, and not mutate it.

Immutability is a powerful concept that helps you to prevent the creation of unexpected side effects in your codebase. It makes it easier for you to read and compose your code.

Since JavaScript is a multi-paradigm language, it does not come with the guarantees that we have in functional programming languages where we can work correctly with the concept of immutability.
```
const car = {
  model: 'Tesla',
  year: 2020
  };

const newCar = car;
  newCar.model = 'Honda';
```

Functional programming is getting more widely used among JavaScript developers, and in this article we learned about a few functional programming concepts that make this paradigm really shine. There is a variety of other concepts in functional programming, but by following the ones that were mentioned here, you will certainly improve your code and skills.

![](https://img.evbuc.com/https%3A%2F%2Fcdn.evbuc.com%2Fimages%2F30423109%2F185617782430%2F1%2Foriginal.jpg?s=e00c5055af924b2c841715f435978f74)









