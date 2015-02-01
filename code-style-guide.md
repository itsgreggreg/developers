The following is a code style-guide that we've found useful in any teaching code we write for the Operation Spark program. We make no claim that this is standard for general development, simply that we've found writing code in this way helpful in avoiding common mistakes and pitfalls. Remember that the #1 priority to be clear and concise so that the kids understand the lesson at hand.

All of these are of course up for debate. If you disagree with one then open it up for discussion in Slack, don't just go your own way.

* **DO** 'use strict' at the top of every script.
* **DO** place all scripts in a `(function() { ... }).call()` IIFE.

* **DO** use double quotes (`"`) as a string delimeter. 
* **DO** declare all variables up front without initialization.
* **DON'T** mix variable declaration, initialization, do stuff, and optionally returning a value within a single function. Reinforce that each function has these areas and that they go in that order.
* **DO** use expression assignment to create functions `myFunc = function() { ... }`.
* **AVOID** anonymous functions. Prefer to assign functions to variables and then pass in those variables into handlers. This is especially the case for multi-line functions.
* **AVOID** chaining jquery methods. We have found that this additional concept can be confusing, especially since it typically involves unusual indentation.

* **DO** use the long-form `[id=foo]`, `[class=bar]` syntax until it becomes convenient to use the short-form `#foo` and `.bar` syntax.
* **AVOID** combining selectors unless specifically teaching that.
* **DO** be fastidious in indenting everything correctly. **AVOID** doing statements on the same line.

* **CONSIDER** using in-page script and style tags until it is helpful to put them in different files.
* **DO** use quotes around html attribute values.

* **AVOID** using the `this` parameter wherever an alternative is available. `this` is a feature that is confusing and poorly understood even by professional developers and the same effect can almost alway be achieved a different way.
     
     var person = {
          name: "Fred Flintstone",
          sayHi: function() {
               return person.name + " says hello";
          }
     }
     $('li').on('click', function(ev) {
           $(ev.target).toggleClass('selected');
     });

* **AVOID** using the `new` keyword. This is even more poorly understood than `this` and even more confusing. With the exception of libraries that force the use of `new` you should avoid it. You do not need its functionality in your own code. You don't. Prefer to extend things directly to share functionality. When you absolutely must use `new` see if you can use the less ambiguous [`Object.create`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/create) instead.
