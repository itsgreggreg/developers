Creating curriculum
==========

Our students run through lessons in a three step process. They first read through the material on a topic in the wiki on Github, then complete an exercise on a browser-based IDE called [Cloud 9](https://c9.io/), and finally take a quiz via a form on Google Docs. The process to create this content is straightforward and we've developed a solid amount in our wiki but there's always more to be done.

For version 1 of our curriculum, we're focusing on JavaScript and HTML5.  Why JavaScript?  Amoung other reasons, JavaScript is ubiquitous: students using our Chromebooks can open up a browser and started building and debugging, without having to install IDE's or compilers, etc.

1. **Material**: Wiki page material on a concept should be readable in under 15 minutes. The page should be written for absolute newbies, and if it's a page on code, list syntax at the top, then a table of contents, then concepts by header.  A table of contents can be automatically generated based on hash (#) headers by using a command-line utility, like doctoc.

   [Check out this example](https://github.com/OperationSpark/variables-and-constants/blob/master/README.md).

   Table of contents generator is [here](https://github.com/thlorenz/doctoc) 

2. **Cloud9 Exercise**: You should provide an exercise with anything that has syntax or markup. Create a simple exercise that practices the concepts outlined in the page.  So, if it's on loops, a simple exercise on JavaScript loops.

3. **Quiz**:  15 questions or less. If applicable, try to break up the quiz into sections using [section headers](https://support.google.com/docs/answer/2839737?hl=en). This will help us give remedial help by targeting weaknesses in that particular area, ie, "you understand what variables are, but you're struggling with keywords, let's go over keywords...". No need to write the quiz from scratch. You can copy the [starter template](https://docs.google.com/forms/d/1MF5h5uIssiqcpy_I-gyOEgLn5VvmT3_XMPqwNtSE_xk/viewform?edit_requested=true) in Google Docs by clicking File > Make a Copy. 

Once you've created the excercise and quiz, go back to the wiki page and add the links to them at the bottom. You'll need to change the hrefs to your wiki page on Github and the "send form" link for the Google Doc form.

Finally, and this is an important step, please take the quiz yourself, answering all questions correctly, so that we have the correct answers in the first row of the "Responses" spreadsheet, against which we can grade quiz responses.

```html
<a href="https://github.com/OperationSpark/variables-and-constants/blob/master/README.md" target="_blank"><img src="https://raw.githubusercontent.com/OperationSpark/javascript-wiki/master/images/btn-code.png" alt="Code a little"></a>

<a href="https://docs.google.com/forms/d/1hV_VWLJDcxHBpzSd63q0WzjrkYI19V9Xz7X8Zh2A8kI/viewform?usp=send_form]" target="_blank"><img src="https://raw.githubusercontent.com/OperationSpark/javascript-wiki/master/images/btn-quiz.png" alt="Take the quiz"></a>
```

<a href="https://github.com/OperationSpark/variables-and-constants/blob/master/README.md" target="_blank"><img src="https://raw.githubusercontent.com/OperationSpark/javascript-wiki/master/images/btn-code.png" alt="Code a little"></a>

<a href="https://docs.google.com/forms/d/1hV_VWLJDcxHBpzSd63q0WzjrkYI19V9Xz7X8Zh2A8kI/viewform?usp=send_form]" target="_blank"><img src="https://raw.githubusercontent.com/OperationSpark/javascript-wiki/master/images/btn-quiz.png" alt="Take the quiz"></a>

Once you're done, please link to your work for review by posting it in the developers channel on [Operation Spark's Slack](https://operationspark.slack.com/). If you don't have a Slack account for Operation Spark yet please email max@operationspark.org to get set up. 

#### State of Wiki

To see what pages are yet to be owned, [open the wiki ownership doc](https://docs.google.com/spreadsheets/d/1k7-oF_8ItWGHWN_CmUzNhqTRuy3g2Bl1-P2JSUoACFM/edit#gid=0).

The [developer playbook](https://docs.google.com/document/d/1iWceCMdFMKs3vRl69VptP0fbnurvtSNVkiUR13-GwSc/edit?usp=sharing) outlines how to write material for the wiki and includes the starter quiz form template.

