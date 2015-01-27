The following is a code style-guide that we've found useful in any teaching code we write for the Operation Spark program. We make no claim that this is standard for general development, simply that we've found writing code in this way helpful in avoiding common mistakes and pitfalls. Remember that the #1 priority to be clear and precise so that the kids understand the lesson at hand.

* **DO** 'use strict' at the top of every script.
* **DO** place all scripts in a `(function() { ... }).call()` IIFE.

* **DO** declare all variables up front without initialization.
* **DON'T** mix variable declaration, initialization, and doing stuff within a single function. Reinforce that each function has these areas.
* **DO** use expression assignment to create functions (`myFunc = function() { ... }`).
* **AVOID** anonymous functions. Prefer to assign functions to variables and then pass in those variables into handlers.
* **AVOID** chaining jquery methods. We have found that this additional concept can be confusing, especially since it typically involves unusual indentation.

* **DO** use the long-form `[id=foo]`, `[class=bar]` syntax until it becomes convenient to use the short-form `#foo` and `.bar` syntax.
* **AVOID** combining selectors unless specifically teaching that.
* **DO** be fastidious in indenting everything correctly. **AVOID** doing statements on the same line.

* **CONSIDER** using in-page script and style tags until it is helpful to put them in different files.
* **DO** use quotes around html attribute values.
