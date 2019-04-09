## Quiz: Reviewing Server Communication

???

# Reviewing Server Communication

?: When we talk about scope in JavaScript, we're talking about:

() how many functions are included in the code.
() how long the code is.
(X) where declared variables and functions are accessible within the code.
() how many variables are declared in the code.

?: What types of scope are there?

[X] function
[X] global
[X] block
[X] local

?: In the following code, we are able to access the myVar value.

```javascript
  function myFunc () {
    const myVar = 25;
  }
  myVar * 5;
```

() True
(X) False

?: It's best practice to create all variables as global variables.

() True
(X) False

?: When the JavaScript engine looks for variable values, it:

() first checks the top of the code for globally declared variables.
() checks another files for declared variables.
(X) first looks for a match locally, then checks outer scopes.
() looks for where the variables are invoked.

?: Scope based on where variables and blocks of scope are defined by the programmer at the time it's written, and solidified by the time the code is processed, is called:

() global scope
(X) lexical scope
() block scope
() nested scope

?: Given the following code sample, what result should we expect to show up in the console?

```javascript
const myVar = 'Foo';

function first () {
  console.log('Inside first()');

  console.log('myVar is currently equal to:', myVar);
}

function second () {
  const myVar = 'Bar';

  first();
}
```

()
// LOG: Inside first()
// LOG: myVar is currently equal to: Bar
// => undefined
(X)
// LOG: Inside first()
// LOG: myVar is currently equal to: Foo
// => undefined
()
// LOG: myVar is currently equal to: Foo
// LOG: myVar is currently equal to: Bar
// => undefined
()
// LOG: Inside first()
// => undefined

?: The following code works just fine. How is it that it can run even though in the code the function declaration happens after the function invocation?

```javascript
myFunc();

function myFunc () {
  return 'Hello, world!';
}
```

(X) The JavaScript engine only cares about function declarations in the compliation phase, and in the execution phase it only cares about function invocations.
() The JavaScript engine can guess what the function is supposed to do.
() The JavaScript engine can physically move your code around to place declarations at the top.
() The JavaScript engine will wait until you declare the function.

?: Best practice in declaring variables is to:

() put all your variables in a separate file.
() repeat your variables in every function.
() make all your variables global.
(X) declare all of your functions at the top of their scope.

?: It is equally okay to use "const," "let," or "var."

() True
(X) FALSE

???
