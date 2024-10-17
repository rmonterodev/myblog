---
layout: post
title:  Prototype Design Pattern
categories: Javascript Design-Patterns
tags: frontend js javascript patterns singleton
---

This design is known as the one that allows us to create objects based on a blueprint/template from an existing object through cloning. In this way we can re-use the properties and methods of the prototype object as well as adding new ones as needed.

In the below example, you can take a look in the main.js file:


**Advantages**

- Save time and memory by copying objects.
- Structured approach to object creation and inheritance.
- Updates in prototype are reflected in all instances.
- Not need to specify all properties and methods during creation, which is easy to initialize.


**Drawbacks**

- Complex and confusing if not used carefully when the application grows.
- Risk of overriding all prototype instances when no intended.
- Weak encapsulation, exposes object properties and methods unintentionally.