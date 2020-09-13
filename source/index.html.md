---
title: FAQ on Java Programming for DDP2

language_tabs: # must be one of https://git.io/vQNgJ
  - java
  - python

toc_footers:
  - <a href='https://scele.cs.ui.ac.id/course/view.php?id=3019'>DDP2 Course Page</a>
  - <a href='https://github.com/MDzkM/DDP2-FAQ/issues'>Report Issues</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - 02start
  - 03firstprogram
  - 04gitflow
  - 05bestpractices

search: true

code_clipboard: true
---

# Introduction

Welcome to the Programming Foundations 2 FAQ website. This site serves to give you an insight on how to start programming with Java and lay down best practices, common pitfalls, and frequently asked questions later down the line. This site's main purpose is to be a companion site for the **Programming Foundations 2 (CSGE601021)** course in Fasilkom UI.



# License and Attribution

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

This website and the corresponding GitHub repository are maintained by:

1. Muhammad Azis Husein
2. Muhammad Dzikra Muzaki
3. Rafi Muhammad Daffa

Any suggestion or feedbacks can be conveyed through the repository's Issues feature.



# Sample Program

Now we are going to create the obligatory `Hello World` code like we do everytime we learn a new language.

> Create this sample program in a file named HelloWorld.java

```java
class HelloWorld {
  public static void main(String args[]) {
    System.out.println("Hello World!");
  }
}
```

# Compiling and Running Program

Now that you've created the template, you can see what output it produces.

> You can run it by compiling it first

```shell
javac HelloWorld.java && java HelloWorld
```
