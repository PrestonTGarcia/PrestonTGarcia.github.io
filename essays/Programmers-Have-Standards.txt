---
layout: essay
type: essay
title: Programmers Have Standards
date: 2021-02-04
labels:
  - Javascript
  - Coding Standards
  - Software Engineering
---

<img class="ui tiny left circular floated image" src="../images/coding-standard.png">

## The Importance of Coding Standards
Coding standards are defined as how we should type up our code, some examples of coding standards are declaring variables according to what they are, making documentation with comments, and how we should type our indents and spacing. Most of the time, not following these coding standards won't have too much affect on whether or not our programs will run or not, or if it will run faster, rather, they're more so about making our programs look more organized and standardized.

So that begs the question: Who cares? Why should we spend our time working on our code's standards, when we could work on other things such as making code efficient, and work better?

<img class="ui tiny left circular floated image"
src="../images/suit.jpg">

## Appearances
I believe that all programmers should have coding standards in mind, as our coding standards help us improve the quality of the code that we program in many ways. The way our code looks is only one way that our coding standards improve code quality. The looks of our code is important as if our code's all unorganized, not only will we not be able to understand our own code when we run into errors, but if we ask for help the organization will lead to others running into trouble as well, as if we don't even think about coding standards our code will be hard to read. Not only that, but much like how our first impression in interviews is how we are dressed, if we post our code up and show it to potential employers, the standards of our code is their first impression on it, as they will see the structure and appearances of our code first.

<img class="ui tiny left circular floated image"
src = "../images/efficiency.png">

## Efficiency and Syntax
Coding standards also help our efficiency in programming, and helps our code run better than if we were to violate many coding standards. Take for example the following class definition from a coding standard exercise in my ICS 314 class.

```Javascript
class MyClass {
  constructor() {}
  getName() {
    return this.name;
  }
  getName() {
    return this.name;
  }
}
```

This code violates coding standards, as it has two identical methods in the class and an empty constructor that the compiler has to read through; however, this code will run just fine if we just trust the compiler. If we were to follow coding standards and fix this code, we have a more efficient code block shown below.

```Javascript
class MyClass {
  getName() {
    return this.name;
  }
}
```

Now, the compiler only needs to read through one method, rahter than two unnecessary ones, improving our efficiency as programmers.

## Conclusion
My ICS 314 professor stated that if we were to improve our code quality by implementing only one software engineering technique, then it should be coding standards. I agree with this, as shown above that implementing coding standards can improve many different aspects of our code, such as looks, efficiency, and syntax. Especially in a weakly typed language such as Javascript, our coding standards will lead us in making higher quality code, rather than unnecessary and unorganized.