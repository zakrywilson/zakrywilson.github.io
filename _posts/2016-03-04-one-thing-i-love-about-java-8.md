---
layout:     post
title:      One small thing I really love about Java 8
date:       2016-03-04 23:44
summary:    A one of the things lambda expressions do to make your life easier
categories: Java
---

## Before 

So before lambda expressions you had to explicitly override the single method. Doing it once isn't much of a problem but when you get a bunch of action listeners in your class, it starts to get pretty cluttered. 

<script src="https://gist.github.com/zakrywilson/ba56966125b02b0c840a.js"></script>

## After

Now, thanks to lambda expressions, if the interface only requires one method to be implemented, you can use a lambda expression. It looks much cleaner… and I love not having the `@Override` annotation.

<script src="https://gist.github.com/zakrywilson/73bcb6169b4954dd1756.js"></script>

See! Way cleaner.
