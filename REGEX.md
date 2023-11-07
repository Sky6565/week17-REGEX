# week17-REGEX

# Regular expressions

The regular expressions, known as regex. A regex is a sequence of characters used to define a search pattern. It is used to validate inputs or used in search algorithms.

## Summary

Using a sample regex and explaining the different aspects of it and what they mean. We will use a sample regex that represents a Google email address:

`/^([\w._%+-]+)@(gmail)+\.([a-zA-Z]{2,4})$/`

While it may look like a bunch of random characters, they all have a specific meaning and are used to make sure strings match the requirements.

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

A regex is composed of multiple parts. It checks to see if a string meets the requirements listed, and the regex is wrapped in slash marks `/`.

### Anchors

The `^` and `$` characters are used as anchors to represent the characters that start and end of a string, respectively. For example, `^Love` means the string must start with "Love" as regexes are case-sensitive.

### Quantifiers

Quantifiers help define how many characters or matches are in a string. They are defined in symbols such as `*` (0 or more matches), `+` (1 or more matches), `?` (0 or 1 matches), or curly brackets. For example, if a section of a regex has to be between 2-4 characters long, then the quantifier will be displayed as `{2,4}`.

### Grouping Constructs

Grouping constructs help break a string into different sections that each have their own requirements. The main way to do so is by using parentheses, so a regex of `(sky)@(gmail)` is looking for a string that contains "sky" followed by an "@" followed by a "gmail."

### Bracket Expressions

Bracket expressions display a range of characters that can be used within a string. They are denoted within square brackets such as `[]`, so if your string must contain a lowercase letter of the alphabet, then the bracket expression will be `[a-z]`.

### Character Classes

A character class is a symbol used to represent a set of characters. For example, `.` means any character except the newline character `\n`. `\d` represents numeric digits. `\w` represents any alphanumeric character as well as the underscore. `\s` represents a whitespace character like a tab or line break.

### The OR Operator

The OR operator `|` denotes that certain characters do not necessarily have to appear in conjunction. For example, an expression of `[x|y|z]` means that the expression can contain x or y or z, not necessarily all three together.

### Flags

Flags are placed at the end of a regex in order to define additional limits for the regex. For example, `g` is used to test the regex against all possible matches. `i` is used to ignore case (uppercase or lowercase) when trying to match a string. `m` treats a multi-line string as multiple lines.

### Character Escapes

A backslash acts as a character escape, which is used to denote a character that would normally be used as a regex component. For example, `\.` denotes the dot character itself and does not signify a character class of `.`.

## Author

This tutorial was written by Godwin To, whose GitHub profile can be found [here](https://github.com/Sky6565)
