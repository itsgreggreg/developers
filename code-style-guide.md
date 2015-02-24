The following is a code style-guide that we've found useful in any teaching code we write for the Operation Spark program. We make no claim that this is standard for general development, simply that we've found writing code in this way helpful in avoiding common mistakes and pitfalls. Remember that the #1 priority to be clear and concise so that the kids understand the lesson at hand.

All of these are of course up for debate. If you disagree with one then open it up for discussion in Slack, don't just go your own way.

* **DO** put "use strict" at the top of every script.
* **DO** place all scripts in a `(function() { ... }).call()`.

* **DO** use double quotes (`"`) as a string delimeter. 
* **DO** declare all variables up front without initialization.
* **DO** always seperate: 
  * variable declaration
  * variable initialization 
  * doing things
  * returning a value
* **DO** Reinforce that each function does these things and that they go in that order.
* **DO** Assign functions to variables `myFunc = function() { ... }`.
* **DON'T** Pass function literals as parameters to functions. It makes the code too hard to read.
* **AVOID** chaining jquery methods. We have found that this additional concept can be confusing, especially since it typically involves unusual indentation.

* **DO** Use full attribute selectors `[id=foo]`, `[class=bar]` until it becomes convenient to use equivalent shorthand selectors `#foo`, `.bar`.
* **AVOID** combining selectors unless specifically teaching that.
* **DO** Be thorough in teaching and enforcing correct indentation. 
* **AVOID** multiple statements on the same line.

* **CONSIDER** using in-page script and style tags until it is helpful to put them in different files.
* **DO** use quotes around html attribute values.

* **AVOID** using `this` wherever possible. `this` is confusing to teach and can usually be avoided.
     
        var person = {
            name: "Fred Flintstone",
            sayHi: function() {
                return person.name + " says hello";
            }
        }
        $('li').on('click', function(ev) {
            $(ev.target).toggleClass('selected');
        });

* **AVOID** using the `new` keyword with the exception of libraries that force you to use it. `new` is even more confusing to teach than `this`. Prefer to extend objects directly to share functionality. When you absolutely must use `new` see if you can use the less ambiguous [`Object.create`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/create) instead.
* **AVOID** Giving variables names that are similar to other things in context. Eg: `html = "<p>" + p.name + "</p>"`
* **DO** Prefer full word variable names over abbreviations. Eg: `person.name` instead of `p.name`
* **AVOID** using plural and singular variable names in the same context. Rather than `players.filter(function(player) {`, consider `allPlayers` and `player`.
