This is a style guide for creating presentations for Operation Spark

* **DO** use slides with a minimal background. White or light gradient. **AVOID** flashy or distracting slides
* **DO** ensure that any project-based lesson is broken into small, discrete, verifiable, and continuous steps
** Small means students shouldn't have to type more than a dozen or so lines of code
** Discrete means that the end of the step should be a logical stopping point. The sort of thing that you might do a commit after.
** Verifiable means that you should provide criteria by which they can verify that they completed that step successfully. Ideally things are visually verifiable but at least have it possible to expose a method on the window object and try invoking it through the console.
** Continuous means that the step should make sense given all the previous steps. We want to avoid the situation where we are putting in code in preparation for a future step before the need for it is obvious to students. This is confusing. Prefer to follow YAGNI principles and refactor afterwards.
* **AVOID** having variable names that are similar to other things that exist in the same context. Eg students tend to find very confusing what is `p` in `html = "<p>" + p.name + "</p>"`
* **AVOID** using plural and singular variable names. Rather than a `players` array and paramters named `player`, consider `allPlayers` and `player`.
