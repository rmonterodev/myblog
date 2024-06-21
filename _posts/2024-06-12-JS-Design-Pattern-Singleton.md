---
layout: post
title:  Singleton Design Pattern
categories: Javascript Design-Patterns
tags: frontend js javascript patterns singleton
---

It's a design that restricts the instantiation of a class to one object. This is useful when only one object is required to be used across the system. This single instance can be used by different parts of the application, which makes Singletons useful for managing global state in an application.

**Singleton** differ from **static classes** because they require cetain data that may not be available during initialization time. 

ES6 allows us to create a global instance of Javascript class that is instantiated once through a module export, making its access to it more explicit and controlled and differentiates it from other global variables. 

It cannot create a new class instance but can read/modify the instance using public get and set previously defined in the class. When attemting to create a new instance, it will simply return a reference of an existent object, if not it will create an instance.

In the below example, you can take a look in the main.js file on how is trying to create a second instance but it automatically returns a reference of the existent instance.

<iframe width="100%" height="800px" src="https://stackblitz.com/edit/vitejs-vite-ulcuwq?embed=1&file=counter.js&theme=dark&view=both&terminalHeight=0"></iframe>

When using the decrement feature, it is trying to use the second instance of counter but it's being inmediately referenced to the unique existent instance.

**Drawbacks**

Because of its simple implementation, we tend to overuse it. Therefore, nowadays, it’s considered to be an anti-pattern. For the following reasons:

- It violates the Single Responsibility Principle. It has at least two responsibilities – making sure only one instance and contains business logic.
- They're global variables, everyone can access them. Moreover, looks they're not inmutable.
- Promotes hidden dependencies and making them hard to test.

**Alternatives**

- Dependency injections.
- Factory Pattern.