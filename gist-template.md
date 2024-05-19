# Regular Expression Tutorial

Understanding Regular Expressions are an integral part of programming and becoming an effective programmer. As a web development students I have developed the following tutorial to help myself and others understand this important Computer Science concept.

## Summary
A Regular Expression or Regex is a seuquence of characters that help define patterns in a string of data that allows to search for data strings that match the pattern such as passwords, email adresses, and URLs for input validation. They are an important part of a programming and computer science.

We will look at the following string of code that is using regex which looks for a matching email:

Ex: ` /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

In the following sections we will be disecting this Regex


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

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

[Alexis Merino](https://github.com/AlexM745)

UTSA Coding Bootcamp Student

## Sources and References
- [MDB_Web_Docs-Regular_Expressions_CheatSheet](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Cheatsheet)
- [MDB_Web_Docs-Regular_Expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions)
- [Coding_Bootcamp-Regex_Tutorial](https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial)
