---
layout: post
title:  Singleton Design Pattern
categories: Javascript Design-Patterns
tags: frontend js javascript patterns singleton
---

It's design that restricts the instantiation of a class to one object. This is useful when only one object is required to be used across the system.

*Singleton* differ from *static classes* because they require cetain data that may not be available during initialization time. 

ES6 allows us to create a global instance of Javascript class that is instantiated once through a module export, making its access to it more explicit and controlled and differentiates it from other global variables. It cannot create a new class instance but can read/modify the instance using public get and set previously defined in the class.