---
layout:     post
title:      A simple Java trick with blocks
date:       2015-11-28 14:58
summary:    Something a surprising amount of Java developers probably don't know
categories: Java
---

### The trick
A lot of Java developers don't know that you can create scopes with named blocks. Not every block needs to be created alongside something such as a loop or a method definition---Java actually allows programmers to define their own scope which can provide programmers some interesting freedom.

### Example
![With brackets](http://i.imgur.com/DQvzs7r.png)

It also works without brackets if you prefer it that way.

![Without brackets](http://i.imgur.com/8qwGSCu.png)

### Disclosure
This would be considered by myself and others as bad programming.

### Then why know this?
I have seen where some Java interviewers will ask about this feature---and also it's just pretty cool.

### Alternative approaches
If you find yourself in a situation like this, try breaking your code up into smaller parts, using `return` statements.
