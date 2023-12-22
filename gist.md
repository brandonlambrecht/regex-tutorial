# Regex Tutorial

A regular expression (regex) is a pattern of characters that defines a specific search pattern. They can be used to validate inputs, replace a character or sequence within a string, and much more. This regex tutorial will breakdown the different elements of a regular expression, how to read a regex, and the proper use for given example listed below.

## Summary

The regular expression being broken down in this repository is an email address validator with the following structure:

- ensures that the email address starts with a valid username followed by an at (@) symbol and a valid domain name
- username can contain lowercase letters, digits, underscores, dots, and hyphens.
- domain name can contain digits,lowercase letters, dots, and hyphens.
- TLD (top level domain) must consist of 2 to 6 lowercase letters or dots.

Here is the regular expression that will be broken down

    - `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Here is an example below:

![Example](regex-example.png)

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

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

- ^ : Declares the start of the string.

- ([a-z0-9_\.-]+) : Capturing group for the username part of the email address. Includes all characters before the @ symbol. The use of the parentheses declares these characters a capturing group.

- ([\da-z\.-]+): Capturing group for the domain name part of the email address:

- ([a-z\.]{2,6}): Capturing group for the top-level domain (TLD):

- [a-z\.]{2,6}: Matches between 2 and 6 of the following characters: lowercase letters (a-z) or dots (.).

- $: Declares the end of the string.

### Anchors

- ^ : Declares the start of the string.
- $ : Declares the end of the string.

### Quantifiers

- +: Matches one or more occurrences of the preceding element.
- {2,6}: Matches between 2 and 6 occurrences of the preceding element.

### Grouping Constructs

- (...) (capturing groups): Used for grouping parts of the expression together for capturing and referencing. - ([a-z0-9_\.-]+) - ([\da-z\.-]+) - ([a-z\.]{2,6})

### Bracket Expressions

- [a-z0-9_\.-]: Matches any single character that is a lowercase letter, digit, underscore, dot, or hyphen.
- [\da-z\.-]: Matches any single character that is a digit, lowercase letter, dot, or hyphen.
- [a-z\.]: Matches any single character that is a lowercase letter or a dot.

### Character Classes

- \d: Matches any digit (equivalent to [0-9]).

### The OR Operator

### Flags

### Character Escapes

## Author

If you have any specific questions or if you'd like further clarification on any of these concepts, feel free to ask!

Please explore my github for a full overview of my [portfolio].

(https://github.com/brandonlambrecht)
