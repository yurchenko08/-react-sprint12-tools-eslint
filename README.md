# React online marathon

## The tasks of the topic "ESLint"

There is some project.

Implement a configuration of `ESLint` for this project to provide next rules:

1. Enforce indent of 4 spaces

	_incorrect code for this rule_
	```js
	if (a) {
	 b = c;
	}
	```
	  
	_correct code for this rule_
	```js
	if (a) {
	    b = c;
	}
	```

2. Require spaces around operators

	_incorrect code for this rule_
	```js
	a=b+c;
	```
	
	_correct code for this rule_
	```js
	a = b + c;
	```

3. Enforce the consistent use of single quotes

	_incorrect code for this rule_
	```js
	a = "double";
	```
	
	_correct code for this rule_
	```js
	a = 'single';
	```

4. Require `let` or `const` instead of `var`

	_incorrect code for this rule_
	```js
	var a = 0;
	```
	
	_correct code for this rule_
	```js
	let a = 0;
	```

5. Require `const` declarations for variables that are never reassigned after declared

	_incorrect code for this rule_
	```js
	let a = 'it`s initialized and never reassigned';
	```
	
	_correct code for this rule_
	```js
	const a = 'it`s initialized and never reassigned';
	```

6. Enforce the use of `===` and `!==`

	_incorrect code for this rule_
	```js
	a == b
	```
	
	_сorrect code for this rule_
	```js
	a === b
	```

7. Disallow the use of `console`

	_incorrect code for this rule_
	```js
	console.log("Some message");
	```

8. Disallow assignment operators in conditional expressions

	_incorrect code for this rule_
	```js
	if (a = 0) {
	  b = c;
	}
	```
	
	_сorrect code for this rule_
	```js
	if (a === 0) {
	  b = c;
	}
	```

9. Disallow unnecessary semicolons

	_incorrect code for this rule_
	```js
	a = b;;
	```
	
	_сorrect code for this rule_
	```js
	a = b;
	```

10. Disallow comments on the same line as code

	_incorrect code for this rule_
	```js
	a = 1; // a to 1
	```
	
	_сorrect code for this rule_
	```js
	// a to 1
	a = 1;
	```

11. Disallow `else` blocks after `return` statements in `if` statements

	_incorrect code for this rule_
	```js
	function demo() {
	  if (a) {
	    return b;
	  } else {
	    return c;
	  }
	}
	```
	
	_сorrect code for this rule_
	```js
	function demo() {
	  if (a) {
	    return b;
	  }
	  return c;
	}
	```
12. The last rule should be defined based on message of the autograding tests.
