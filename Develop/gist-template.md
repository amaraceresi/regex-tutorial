# Understanding Regex: Email Validation

Regex, short for regular expressions, are used to find specific patterns in strings. In this tutorial, we will break down a regex used for basic email validation

## Summary

This regex /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is used to validate an email address with a common format, something like name@domain.com.

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

### Anchors

Anchors are `^` and `$` in our regex. 

`^` marks the start of the line 

and `$` marks the end of the line.

### Quantifiers

Quantifiers determine how many instances of a character, group, or character class must be present in the input for a match to be found. 

In our regex, `+` and `{2,6}` are quantifiers. 

`+` matches one or more of the preceding character 

and `{2,6}` matches between 2 and 6 of the preceding character.


### Grouping Constructs

Grouping constructs are `()` in our regex. 

They capture the characters matched for use with other parts of the regex.


### Bracket Expressions

Bracket expressions are `[]` in our regex. 

They define a set of characters of which only one need to be matched.

### Character Classes

Character classes represent a set of characters. 

In our regex, `[a-z0-9_\.-]` and `[\da-z\.-]` are character classes. 

`[a-z0-9_\.-]` matches any lowercase letter, any digit, underscore, period or dash, 

and `[\da-z\.-]` matches any digit, lowercase letter, period or dash.


### The OR Operator

The OR operator in regex is represented by the pipe symbol `|`. It allows the regex to match the pattern before or the pattern after the operator.

For example, in the regex `(cat|dog)`, the regex will match either "cat" or "dog".


### Flags

Flags are used in regex to control the matching behavior of the regex. They follow the closing slash of the pattern.

For example, the `g` flag makes the regex search for all matches in the input string, not just the first match. The `i` flag makes the regex case insensitive.

In our email regex, we do not use any flags.

### Character Escapes

Character escapes are used when you want to match a character that has special meaning in regex, such as `.` (dot). 

You can escape it with a backslash `\\.` to tell the regex you want to match the actual dot character.


## Author

This tutorial was created by Amara Ceresi. Feel free to reach out with any questions.

## GitHub

https://github.com/amaraceresi




