---
title: "let and const keywords in ES6"
date: 2022-12-25T09:05:15-05:00
draft: false
---

`let` and `const` are new keywords introduced in `ES6` which enable us to change the way we work with variables and constants. Let and const are both block scoped. Prior to `ES6`, we had only function scope and global scope. Block scope restricts variable access to blocks, i.e. constructs with curly braces, such as `if...else`, `for loops`, etc. As an example:

In the past, we would declare variables using var as follows:

```javascript
if(true){
  var age = 23
}
console.log(age);
```

But with `ES6`, if we now use let to declare a variable inside a block of code, it fails with a legitimate error: 

```javascript
if(true){
  let age = 23
}
console.log(age);
```

Code block above fails with an error such as: 

```
"error"
"ReferenceError: age is not defined
    at yozibopigo.js:9:38
    at https://static.jsbin.com/js/prod/runner-4.1.8.min.js:1:13924
    at https://static.jsbin.com/js/prod/runner-4.1.8.min.js:1:10866"

```

You can read more about scopes [here](https://developer.mozilla.org/en-US/docs/Glossary/Scope). 