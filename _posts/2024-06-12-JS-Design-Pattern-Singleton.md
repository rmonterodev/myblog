---
layout: post
title:  Singleton Design Pattern
categories: Javascript Design-Patterns
tags: frontend js javascript patterns singleton
---

It's a design that restricts the instantiation of a class to one object. This is useful when only one object is required to be used across the system. This single instance can be used by different parts of the application, which makes Singletons useful for managing global state in an application.

**Singleton** differ from **static classes** because they require cetain data that may not be available during initialization time. 

ES6 allows us to create a global instance of Javascript class that is instantiated once through a module export, making its access to it more explicit and controlled and differentiates it from other global variables. It cannot create a new class instance but can read/modify the instance using public get and set previously defined in the class. When attemting to create a new instance, it will simply return a reference of an existent object, if not it will create an instance.