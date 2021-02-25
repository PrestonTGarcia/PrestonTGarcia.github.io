---
layout: essay
type: essay
title: Simple but Difficult
# All dates must be YYYY-MM-DD format!
date: 2021-02-25
labels:
  - Software Engineering
  - UI Frameworks
  - HTML
  - Semantic UI
---

<img class="ui fluid image" src="../images/semantic.png" alt="semantic image">

## Semantic UI

Recently, I've been learning how to use Semantic UI with a little bit of CSS to create webpages rather than using just raw HTML and CSS. When I was first started learning Semantic UI, it was said in the course that Semantic UI uses "natural language", or more English rather than actual code. An example of the difference between Semantic UI and raw HTML and CSS when creating columns in webpages is shown below.

### Semantic UI Code

```HTML
<div class="ui grid">
	<div class="column">Column 1</div>
	<div class="column">Column 2</div>
	<div class="column">Column 3</div>
</div>
```

### Raw HTML and CSS code
```HTML
<div class="left">Column 1</div>
<div class="center">Column 2</div>
<div class="right">Column 3</div>
```

```CSS
.left{
	float: left;
	width: 300px;
}
.center{
	margin-left: 300px;
	margin-right: 300px;
}
.right{
	float: right;
	width: 300px;
}
```

After hearing about this simplicity and natural language, my first thought was "Wow, Semantic UI is super convenient, and is gonna be a piece of cake". I was far from correct, as regardles of its simplicity, learning Semantic UI was just as difficult as learning a whole new programming language. This begs the question: is learning Semantic UI over HTML and CSS worth the difficulty? In my opinion, the benefits of Semantic UI such as its predictability and simplicity outweigh the difficulties of learning Semantic UI.

<img class="ui tiny left circular floated image" src="../images/documentation.png" alt="documentation image">

## Predictability

Semantic UI has predictability in two ways, predictability in syntax, and predictability in what code creates a certain part of a webpage. Since most of the syntax uses natural English language, the modifiers for class names can be predicted easily sometimes. For example, if we were creating a menu, for each item in it the class name would just have an "item" at the end of it. If we wanted the item to be a dropdown menu, we can just call the class "dropdown item", and even if the modifiers can't just be predicted Semantic UI has great documentation to use. With this documentation, they provide many examples of what code can create different visuals, giving predictability of what the webpages will look like, while raw HTML and CSS doesn't have much visual documentation. 

<img class="ui tiny left circular floated image" src="../images/simplicity.jpg" alt="simplicity image">

## Simplicity

Looking at the code shown comparing Semantic UI to raw HTML and CSS, it's easy to see how much more simple the Semantic UI components are. The Semantic UI code requires only 5 lines of HTML, while the raw HTML and CSS required 3 lines of HTML and 12 lines of CSS in order to do the same thing. The raw HTML and CSS is also not dynamic with different screen sizes like Semantic UI is. This simplicity of the code helps far more than expected, as it allows us to focus more on the organization and coding standards of our code, which will go a long way. 

## Conclusion

Semantic UI is just like any other external programming language, or even engineering and physics as while it is difficult to learn and perform sometimes, it allows us to perform more efficiently. Semantic UI has benefits of predictability with its natural language and documentaiton, and simplicity with its improvement of organization and coding standards.  