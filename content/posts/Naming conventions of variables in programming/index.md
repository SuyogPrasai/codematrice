---
title: "Naming conventions of variables in programming"
subtitle: "Naming conventions of variables in programming"
date: 2023-12-04T16:54:39+05:45
lastmod: 
draft: false 
author: "Suyog Prasai"
authorLink: ""
description: "In this post, I will be talking about the various naming conventions that we use to name variables, classes, functions, etc. I hope that this is particularly useful to those who are new in this."
license: ""
images: []

tags: ["blog", "programming"]
categories: ["blog"]

featuredImage: "cover.webp"
featuredImagePreview: ""

hiddenFromHomePage: false
hiddenFromSearch: false
twemoji: false
lightgallery: true
ruby: true
fraction: true
fontawesome: true
linkToMarkdown: false
rssFullText: false

toc:
  enable: true
  auto: true
code:
  copy: true
  maxShownLines: 50
math:
  enable: false
  # ...
mapbox:
  # ...
share:
  enable: true
  # ...
comment:
  enable: true
  # ...
library:
  css:
    # someCSS = "some.css"
    # located in "assets/"
    # Or
    # someCSS = "https://cdn.example.com/some.css"
  js:
    # someJS = "some.js"
    # located in "assets/"
    # Or
    # someJS = "https://cdn.example.com/some.js"
seo:
  images: []
  # ...
---

## Naming Conventions

Naming conventions refer to the **guidelines** that we as programmers follow to name various identifiers like **variables**, **functions**, **class**, etc. This is particularly useful when we need to find a specific thing (e.g., variable, function, or even files). This makes us more productive as programmers and helps us to identify what is what.

<!--more-->

### Why do we need them?

As I said earlier, **naming conventions** are very useful and are a standard of professional developers. We, as developers, are constantly reading and writing code in our domain. This makes us encounter different types of code and logic. If we are able to identify what is what, then we can more easily comprehend the program. If we are able to do this, then it becomes very easy for us to add features, remove features, refactor code, and many more.

{{< admonition type=tip title="Some points to remember" open=true >}}
1. Giving good names to identifiers makes it easy to find things.
2. Which, in return, gives us more comprehension of the code and logic.
3. This makes us more effective as programmers and greatly improves our skill.
4. It also helps us to differentiate if something is to be accessible to the user and what is to be used within the function (abstraction).
{{< /admonition >}}

### Naming Conventions across programming

Now that we understand why naming conventions are important in our field, we can dive into the various _naming conventions_ that are actually used.

These are different case notations that you will come across while programming. It is better to remember them all (it is quite useful).

1. **Camel Case:**
   - Example: `camelCaseVariable`
   - In camel case, the first letter of each word is capitalized except for the first word.

2. **Pascal Case (or Upper Camel Case):**
   - Example: `PascalCaseVariable`
   - Similar to camel case, but the first letter of the first word is also capitalized.

3. **Snake Case:**
   - Example: `snake_case_variable`
   - Words are separated by underscores, and all letters are usually lowercase.

4. **Kebab Case (or Dash Case):**
   - Example: `kebab-case-variable`
   - Words are separated by hyphens, and all letters are usually lowercase.

Now that you know about the various case notations, I can show you what you should do to define an identifier (at least a general guideline).

1. **Be descriptive about your identifiers:**
   - You should be descriptive about your identifiers which gives you info on what is what and what does what. This is a general rule of thumb. For example, "backgroundSetter" can be a name of a function that sets the background of your desktop. Similarly, you should try to use names that actually describe what the function does.

2. **Use camel case or snake case:**
   - For variable and function use either camel case or snake case. I generally use snake case for variable names and camel case for variables. That is my style, but you can be free to choose whether to use camel or snake case.

3. **Avoid Single-letter names:**
   - It is often tempting to use single-letter names to define variables such as counters in a loop, but in production code, that is rarely seen. This is because when the codebase gets bigger and bigger, it becomes increasingly difficult for us to debug code and understand it better. So, try to avoid this pattern.

4. **Consistency is Key:**
   - Maintain a consistent naming style throughout your codebase. If you start with a particular convention, stick to it.

5. **Consider the Scope:**
   - Use longer and more descriptive names for variables with larger scopes (e.g., class-level variables) and shorter names for local variables.

6. **Follow Language Conventions:**
   - Adhere to the naming conventions established by the programming language you're using.

7. **Use Verb-Noun Naming for Functions:**
   - Choose function names that indicate actions. For example, calculateTotal, getUserData.

8. **Think about the Future:**
   - Consider how maintainable your code will be in the future. Choose names that will still make sense as the code evolves.

9. **Review and Refactor:**
   - Regularly review your code and refactor names if needed. As your understanding of the code improves, you may find better names.

10. **Documentation:**
    - If an identifier's purpose is not immediately clear from its name, consider adding comments or documentation to explain its role.

## Conclusion

In essence, naming conventions are the unsung heroes of clean and maintainable code. By adhering to well-established guidelines such as Camel Case or Snake Case, developers create a shared vocabulary that enhances code readability and collaboration. Thoughtful and descriptive identifiers serve as beacons, guiding programmers through the logic of a program and facilitating seamless code maintenance. Consistency in naming not only streamlines individual projects but also fosters a universal language in the programming community. Embracing these conventions is akin to investing in the longevity and clarity of code, ultimately contributing to more efficient development and a collective pursuit of code quality.
