---
layout: post
title:  "CSS preprocessors - pros and cons"
date:   2018-11-17 01:26:26 -0600
categories: jekyll update
---

{% comment %}
  TODO: update this post; it is currently incomplete.
{% endcomment %}

## What are CSS preprocessors?
A CSS-preprocessor is an application which acts as an extension to regular CSS by adding additional functionality and abstractions. The output is compiled into regular CSS that can be delivered to the browser.


### Advantages to regular CSS
Abstraction makes life easier! Most CSS preprocessors offers a number of features such as:
- Variables
- Nesting
- Partials
- Mixins
- Internal functions, for example for handling colors.

What this does is that it gives us as developers some direct advantages such as:
- Easier maintainabilty
- More customizable code
- More DRY - we can re-use partials and mixins to avoid repeating code


### Cons
There are arguably some cons of using a CSS preprocessor. Some of the most obvious include:
- Increased version control complexity: should the compiled CSS be included in repos? If we decide to include the compiled CSS in our repos, we need to make sure that all develpers involved in the project understands the correct work-flow, or risking that someone edits the compiled CSS directly, instead of the input that is fed to the CSS preprocessor.
- Learning curve; developers need to learn new syntax
- Additional tooling is required to compile into CSS
- Harder to debug - since the CSS is compiled we have no way of accessing the variables which generated the CSS. However there are tools to solve this issue.

However, I would agree that the pros outweighs the cons by far!
