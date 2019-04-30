---
layout: "post"
title: "Abstract Class: What and Why "
date: 2019-04-08 17:55:00 -0700
---

## What is Abstract Class
In programming languages, an abstract type is a type in a nominative type system that cannot be instantiated directly; a type that is not abstract – which can be instantiated – is called a concrete type. Every instance of an abstract type is an instance of some concrete subtype.

## Why Abstract Class?

Consider using abstract classes if any of these statements apply to your situation:

- You want to share code among several closely related classes.
- You expect that classes that extend your abstract class have many common methods or fields or require access modifiers other than public (such as protected and private).
- You want to declare non-static or non-final fields. This enables you to define methods that can access and modify the state of the object to which they belong.
