1. What is event bubbling?
2. What is a promise?
3. What is closure?
4. What are event loops?
5. What is a callback?
6. What's the difference between == and ===?
  * == checks for value only. === checks for value AND type
  * '2' == 2 // returns true, because they are equal in value
  * '2' === 2 // returns false because one is a string and the other is an integer
7. Context-binding:
  - this
  - call
  - apply
  - bind
8. What is function currying?
9. Explain prototypal inheritance
  - Every object is associated with some other object, known as its prototype. The last prototype in this "prototype chain" will be equal to null.
  -In terms of inheritence, JavaScript will traverse the prototype chain until it finds the referenced property.
10. Explain constructor functions (specific examples)
11. OOP
12. What is NaN?
  - NaN stands for "Not a Number"
  - type is Number `typeof NaN === 'number'`
  - NaN compared to anything is false (even itself) `console.log(NaN === NaN) // logs false`
  - To check if a value is NaN, you can check for its inequality to itself. `var a = NaN; a !== a; //true`
13. Why would you put 'use strict' at the beginning of your file or function?
14. Be aware of limitations of precisions in JavaScript's double-precision floating-point arithmetic

