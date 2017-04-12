## 1) Describe a closure in JavaScript.

## 2) Returning an inner function does not call the function when the outer function is called. How can this be resolved?

## 3) In the example below, why does the global variable get reassigned?
var reassignmentExample = "Global variable";

function testAssignment() {
  reassignmentExample = "Local variable";

  console.log(reassignmentExample);     
}

console.log(reassignmentExample); // Logs: Global variable

testAssignment(); // Logs: Local variable

console.log(reassignmentExample); // Logs: Local variable (the global variable is reassigned)

## 4) When would it be necessary to store the value of this in a variable?

## 5) Describe the difference between function scoping and block scoping.

## 6) In this example, why does logging 'hoistedVar' return 'undefined'?
function hoistingExample() {

  console.log(hoistedVar);

  var hoistedVar = "Hoist me!";
}
