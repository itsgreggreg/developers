The following is a presentation style-guide that we've found useful in any teaching code we write for the Operation Spark program. We make no claim that this is a standard for presentations or development in general, simply that we've found writing presentations in this way helpful in avoiding common mistakes and pitfalls. Remember that the #1 priority to be clear and concise so that the kids understand the lesson at hand.

All of these are of course up for debate. If you disagree with one then open it up for discussion in Slack, don't just go your own way.

* **DO** use slides with a minimal background. White or light gradient. **AVOID** flashy or distracting slides
* **DO** ensure that any project-based lesson is broken into small, discrete, verifiable, and continuous steps
  * Small means students shouldn't have to type more than a dozen or so lines of code
  * Discrete means that the end of the step should be a logical stopping point. The sort of thing that you might do a commit after.
  * Verifiable means that you should provide criteria by which they can verify that they completed that step successfully. Ideally things are visually verifiable but at least have it possible to expose a method on the window object and try invoking it through the console.
  * Continuous means that the step should make sense given all the previous steps. We want to avoid the situation where we are putting in code in preparation for a future step before the need for it is obvious to students. This is confusing. Prefer to follow YAGNI principles and refactor afterwards.
**DO** create code templates taht can be cloned from Github. We are there for a limited amout of time and not everyone is great at typing. **AVOID** creating lessons where a significant amount of classtime will be blown typing things that students don't understand or are tangerial to the lesson at hand.
**DO** put clear and exclit instructions on how to clone and get started in your slides.
**CONSIDER** including a mockup for project-based lessons. Operation Spark has a Balsamiq license.
**DO NOT** spend a lot of time lecturing on syntax. Concepts are way more important.
