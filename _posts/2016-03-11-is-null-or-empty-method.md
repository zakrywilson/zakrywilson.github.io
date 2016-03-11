---
layout:     post
title:      Tired of constantly checking if strings are null or empty?
date:       2016-03-11 10:02
summary:    A simple solution to redundant code
categories: Java
---

## The problem

I'm sure we all have seen something like this a million times.

{% highlight java %}
if (myString != null && !myString.equals("")) {
    // Do stuff
}
{% endhighlight %}

You have a string that was initialized to null, but then there is also a case where it might be empty. This can sometimes result if you having to check multiple fields to ensure that you have correct data.

{% highlight java %}
if ((a != null && !a.equals("")) && 
    (b != null && !b.equals(""))) {
    // Do stuff
}
{% endhighlight %}

Right? We all know what this is like, more or less.

## A nice solution

Here is a great way to beat the redundancy.

{% highlight java %}
public static boolean isNullOrEmpty(String... strings) {
    for (String string : strings) {
        if  (string == null || string.equals(""))
            return true;
        } 
    return false;
}
{% endhighlight %}

Now let's look at the difference.

{% highlight java %}
if (isNullOrEmpty(a, b)) {
    // Do stuff
}
{% endhighlight %}

Not ground-breaking, but it might just make things a little easier and cleaner.
