---
layout: post
title:  Module Design Pattern
categories: Javascript Design-Patterns
tags: frontend js javascript patterns
---

This a great way to keep project code cleanly separated and organized by different categories. It would help a lot a team of developers to browse between a bunch of files in order to reach a specific funcionality to add or improve.

In the book mentioned 4 options for implementing modules:

- Object Literal Notation.
- The Module Pattern.
- AMD modules.
- CommonJs modules.

We will to look a those 4 deeply in the next sections:

*Object Literals*

It's an object described as a simple set of comma-separated names and values pairs enclosed in curly braces ({}). See below example:

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="XWwbWzE" data-editable="true" data-user="rmontero90" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/rmontero90/pen/XWwbWzE">
  Module Pattern</a> by Rafael Montero (<a href="https://codepen.io/rmontero90">@rmontero90</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

<br />
*Module Pattern*

It is defined to provide private and public encapsulation for objects, functions, classes or variables. It wraps them protecting pieces from leaking into the global scope or accidentally colliding with another developer's interface. 

With this pattern, it will allow us to expose only the public API keeping everything else within the closure private.

Here we have an example for this:

<iframe width="100%" height="300px" src="https://stackblitz.com/edit/stackblitz-starters-c79uwj?embed=1&file=myModule.js&theme=dark&view=both&terminalHeight=0"></iframe>