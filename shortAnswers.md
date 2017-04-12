## 1) Describe a closure in JavaScript.
  A closure in JavaScript is is the combination of a function and the lexical environment within which that function was declared.

## 2) Returning an inner function does not call the function when the outer function is called. How can this be resolved?
This can be fixed by returning the inner function inside of the outside function.

## 3) In the example below, why does the global variable get reassigned?
var reassignmentExample = "Global variable";

function testAssignment() {
  reassignmentExample = "Local variable";

  console.log(reassignmentExample);     
}

console.log(reassignmentExample); // Logs: Global variable

testAssignment(); // Logs: Local variable

console.log(reassignmentExample); // Logs: Local variable (the global variable is reassigned)

**The global variable gets reassigned because the value was changed inside of the function. Then the function was called and that is what changed the variable.**

## 4) When would it be necessary to store the value of this in a variable?
In order to obtain the invocation context of the outer function using this it would need to be added into a variable.

## 5) Describe the difference between function scoping and block scoping.
Function scoping is basically just the scope of the function where as block scoping is the scope of a loop or an in statement.

## 6) In this example, why does logging 'hoistedVar' return 'undefined'?
function hoistingExample() {

  console.log(hoistedVar);

  var hoistedVar = "Hoist me!";
}
**The reason hoistedVar is undefined is because it is not defined before it is called. hoisting does not work on variables when it is inside of the function.**
