# Matching an Email - Regex Tutorial


This tutorial will introduce Regular Expressions and explain how to match emails. Perhaps the greatest advantage of using Regex is its accuracy - regular expressions can accurately match the pattern of a valid email address. Thus, if email addresses pass regex validation then they are likely to be legitimate and valid.


## Summary


In this tutorial, we will use the following regular expression: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. This tutorial will explain the regex components pertaining to it so that it can be simplified and easier to understand.


## Table of Contents


- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components


### Anchors


In this regular expression for matching an email we use the following two anchors: `^ ` and `$`. As for `^`, it indicates the beginning of a string. Whereas, `$` indicates the end of the string. As the word "anchor" suggests, we set these two anchors for our regex expression and place the necessary elements between them.


### Quantifiers


Quantifiers are used to specify the quantity of characters or symbols. In a regular expression, quantifiers will determine exactly how many times a particular element should be matched in the input string. In our regular expression for example, `+` and `{2,6}` are the two quantifiers.


As for `+`, it is used twice in our regex expression; `[a-z0-9_\.-]+` and `[\da-z\.-]+`. In both instances, it specifies that each character matching those inside the brackets is expected to appear at least once.


As for the `{2,6}` quantifier, it will match a domain extension with a minimum character length of two characters and a maximum character length of six characters. This will ensure that our domain extension is within a certain range of characters such as "co", "com", "blog", "co.uk", etc.


### Character Classes


The `\d` character class in this expression will match any single character that is a digit from 0-9. The backslash is used to represent a predefined character class in regular expressions. Here, we set the shorthand for matching digits from 0-9 but in `([\da-z\.-]+)` it is used to match one or more occurrences of these characters after the '@' symbol, but before the domain extension.


### Grouping and Capturing


In regex, parenthesis conveniently indicate groupings. In our expression, there are three groupings. Since email addresses have three components - a string, followed by a website, followed by a domain, it is understandable why the expression should be grouped into three sections.


### Bracket Expressions


Square brackets `[]` denotes bracket expressions. They define a set of characters that can be matched at a specific position in the input string. Any character within the square brackets can be a potential match for that position. As for our code there are three instances: `[a-z0-9_.-]`, `[\da-z.-]`, and `[a-z.]`.


As in the first instance, `[a-z0-9_.-]` will match any lowercase letters from a-z, any digit from 0-9, dot, or hyphen.


## Author


You can find my projects at https://github.com/abasit96?tab=repositories.

