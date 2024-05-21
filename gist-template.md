# Regular Expression Tutorial

Understanding Regular Expressions are an integral part of programming and becoming an effective programmer. As a web development students I have developed the following tutorial to help myself and others understand this important Computer Science concept.

## Summary

A Regular Expression or Regex is a seuquence of characters that help define patterns in a string of data that allows to search for data strings that match the pattern such as passwords, email adresses, and URLs for input validation. They are an important part of a programming and computer science.

We will look at the following string of code that is using regex which looks for a matching email:

Ex: ` /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

In the following sections we will be dissecting this regex.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

A Regular Expressions in JavaScripit has two ways of being created. Either by using a literal where the pattern of characters is wrapped by slashes `/a#b+c/`,and the other by calling the RegExp constructor that use quotation marks `RegExp("a#b+c");`.

For this tutorial we will look at the "Matching Email" regex, you will see the pattern start and end with a foward slash.:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Lets look at the compents of this Regular Expression.

### Anchors

The caret(^) the dollar ($) are characters with special meaning because they are called "anchors" in regular expressions. They do not match a character but they tell the regex engine to check the condition.

* `^` matches the start of the string with the characters that follow it.

    - An exact match of the string will work but you have to be careful because regex are **case-senstive**.

 * `$` matches the end of the string with the characters that before it.

Both of them can have a range of possible matches which are displayed with brackets which will be explain in the a following [section](#bracket-expressions).

In the "Matching Email" regex, the string has to start and finish with something that matches
the following patterns:`^([a-z0-9_\.-]+)`and the`([a-z\.]{2,6})$`.  

### Grouping Constructs

Now that we know how to set the start and the end of our regex. We can now look at the next part of it, which are the parentheses`()` and they are a grouping construct.

Grouping contructs have two categories capturing and non-capturing. Our regex is a capturing group because it does not include the following characters`?:`at the start in the parentheses.

Parentheses are the primary way of grouping sections in a regex and anything within the `()` are called subexpressions. 
In our regex we have 3 grouping constructs:

"/^`([a-z0-9_\.-]+)`@ `([\da-z\.-]+)`\.`([a-z\.]{2,6})`$/". 

* The first subexpression is looking to capture the match of the username of the email address which has the @ symbol after it for the email server.

* The second subexpression is looking to capture the match of the email server which has the "." after it for the domian.

* The third subexpression is looking to capture the match of the domain which is the end of our regex.

### Bracket Expressions

### Quantifiers
Quantifiers specify the number of characters or section of string to match. They might include minimum and maximum numbers of characters for your regular expression. 

Our regex has two quantifiers the plus sign `+` and curly brackets`{}`.
    - `+` matches the pattern one or more times
    - `{}` can provide 3 different ways to set limits.

In our regex we see the `+` operator twice in the first two subexpressions:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\`.

The `+` which is inside the parentheses connects the username + email server + domain (Ex:`.com`).

The curly brackets are at the end of our regex in the third subexpression inside the parentheses: `([a-z\.]{2,6})`.

The curly brackets in our regex are setting the limit of matching the mininum number of 2 and the maximum number of 6 characters for the character set of `[a-z\.]`.

### Character Classes

### Character Escapes


## Author

[Alexis Merino](https://github.com/AlexM745)

UTSA Coding Bootcamp Student

## Sources and References
- [MDB_Web_Docs-Regular_Expressions_CheatSheet](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Cheatsheet)
- [MDB_Web_Docs-Regular_Expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions)
- [Coding_Bootcamp-Regex_Tutorial](https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial)
