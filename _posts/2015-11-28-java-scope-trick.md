---
layout:     post
title:      A simple Java trick with blocks
date:       2015-11-28 14:58
summary:    Something a surprising amount of Java developers don't know
categories: Java
---

### The thing
A lot of Java developers don't know that you can
create scopes with named blocks. Not every block 
needs to be created alongside something such as a 
loop or a method definition---Java actually allows
programmers to define their own scope which can
give programmers some interesting freedom.

### Example
![Blocks and scope](http://i.imgur.com/eIW8cej.png)

### Disclosure
This would be considered by myself and others
as bad programming.

### Then why know this?
I have seen where some Java interviewers will ask about
this feature---and also it's just pretty cool.

### Alternative approaches
If you find yourself in a situation like this, try
breaking your code up into smaller parts, using 
`return` statements.