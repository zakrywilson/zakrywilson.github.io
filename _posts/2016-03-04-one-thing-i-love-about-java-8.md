---
layout:     post
title:      One small thing I really love about Java 8
date:       2016-03-04 23:44
summary:    A one of the things lambda expressions do to make your life easier
categories: Java
---

## Before 

So before lambda expressions you had to explicitly override the single method. Doing it once isn't much of a problem but when you get a bunch of action listeners in your class, it starts to get pretty cluttered. 

{% highlight java %}
button.addActionListener(new ActionListener() {

  @Override
  public void actionPerformed(ActionEvent event) {
    doWhatButtonsDo();
  }
  
});
{% endhighlight %}

## After

Now, thanks to lambda expressions, if the interface only requires one method to be implemented, you can use a lambda expression. It looks much cleaner… and I love not having the `@Override` annotation.

{% highlight java %}
button.addActionListener(event -> {
  doWhatButtonsDo();
});
{% endhighlight %}

See! Way cleaner.
