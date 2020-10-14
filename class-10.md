# Class 10

## Error Handling & Debugging

The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it.

Each execution context can also access its parent's variables object. If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code. If none is found, it continues to the next level, checking to see if here is code to handle the error in that execution context. It can continue until it reaches the global context, where it would have to it terminate the script, and create an Error object.

Error objects can help you find where your mistakes are and browsers have tools to help you read them.

The table below shows the error object properties and their description:

| Property | Description |
|----|----|
| name | Type of execution |
| message | Description |
| fileNumber | Name of the JavaScript file |
| lineNumber | Line number of error |

The table below shows seven different types of built-in error objects in JavaScript and theit description:

| OBJECT | DESCRIPTION |
|----|----|
| Error | Generic error - the other errors are all based upon this error |
| Syntax Error | Syntax has not been followed |
| ReferenceError | Tried to reference a variable that is not declared/within scope |
| TypeError | An unexpected data type that cannot be coerced |
| Range Error | Numbers not in acceptable range |
| URI Error | encodeURI ().decodeURI(), and similar methods used incorrectly |
| EvalError | eval() function used incorrectly |

### Dealing with errors

There are two things you can do with the errors:

1. Debug the script to fix erros.
2. Handle errors gracefully

### Debugging

Debugging is about deduction by eliminating potential causes of an error. The first step in debugging is asking the question 'Where is the problem?` and that could be answered with the help of the browsers dev tools where error messages can be found. The second question after knowing where the problom is 'What is the problem?' and that could be discovered by observing the line of code where the problem occured and search for missing parameters, syntax errors or any other possible error.

### Handling Exceptions

Thiis method is used when you know your code might fail for one reason or another. In this case, it's better to use this method is shown in the block of code below:

```javascript
try {
    // Try to execute this code
} catch (exception) {
    // If there is an exception, run this code
} finally {
    // This always gets executed
}
```

The list below shows a set of common errors you should take into consideration when debugging:

1. JavaScript is case sensitive so check your capitalization.
2. If you did not use var to declare the variable, it will be a global variable, and its value could be overwritten elsewhere (either in your script or by another script that is included in the page).
3. If you cannot access a variable's value, check if it is out of scope.
4. Do not use reserved words or dashes in variable names.
5. Check that your single I double quotes match properly.
6. Check that you have escaped quotes in variable values.
7. Check in the HTML that va lues of your id attributes are unique.
8. Every statement should end in a semicolon.
9. Check that there are no missing closing braces } or parentheses ).
10. Check that there are no commas inside a , } or , ) by accident.
11. Always use parentheses tosurround a condition that you are testing.
12. Check the script is not missing a parameter when calling a function.
13. undefined is not the same as null : null is for objects, undefined is for properties, methods, or variables.
14. Check that your script has loaded.
15. Look for conflicts between different script files.
16. Using= rather than == will assign a value to a variable, not check that the values match.
17. If you are checking whether values match, try to use strict comparison to check datatypes at the same time. (Use === rather than ==.)
18. Inside a switch statement. the values are not loosely typed (so their type will not be coerced).
19. Once there is a match in a switch statement, all expressions will be executed until the next break or return statement is executed.
20. The replace() method only replaces the first match. If you want to replace all occurrences, use the global flag.
21. If you are using the parseInt() method, you might need to pass a radix (the number of unique digits including zero used to represent the number).

The list below shows a set of common debugging tips that help developers:

1. ANOTHER BROWSER
Some problems are browserspecific.
Try the code in another
browser to see which ones are
causing a problem.
2. ADD NUMBERS: Write numbers to the console so you can see which the items get logged. It shows how far your code runs before errors stop it.
3. STRIP IT BACK: Remove parts of code, and strip it down to the minimum you need. You can do this either by removing the code altogether, or by just commenting it out using multi-line comments.
4. EXPLAINING THE CODE: Programmers often report finding a solution to a problem while explaining the code to someone else.
5. SEARCH: Stack Overflow is a Q+A site for programmers. Or use a traditional search engine such as Google, Bing, or DuckDuckGo.
6. CODE PLAYGROUNDS: If you want to ask about  problematic code on a forum, in addition to pasting the code into a post, you could add it to a code playground site (such as JSBin.com, JSFiddle.com, or Dabblet.com) and then post a link to it from the forum. (Other popular playgrounds include CSSDeck.com and CodePen.com - but these sites place more emphasis on show and tell.)
7. VALIDATION TOOLS: There are a number of online validation tools that can help you try to find errors in your code:
    * JAVASCRIPT: <http://www.jslint.com> or <http://www.jshint> .com
    * JSON: http:// www.jsonlint.com
    * JQUERY: There is a jQuery debugger plugin available for Chrome which can be found in the Chrome web store.

[Back to Home](README.md)
