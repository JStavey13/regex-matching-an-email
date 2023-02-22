# Title (replace with your title)

Welcome to my Gist! In this gist I will breakdown a regular expression (regex) and show you how it works piece by piece. This particular regex will be 
used for matching an email address in a string of text.

## Summary


The following snippet of code is a regex used to match an email address. I will explain what each character does sequentially and how they all fit together to do something cool.
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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
the language of a regex is broken up into several sub categories outlined below.

### Anchors
anchors are used to orient oneself within a regex. For example, the ^ matches a string that includes all of the characters that follow it, and the $ matches all of the characters that precede it. In this case, the ^ and $ encompass the whole regex, showing that we are only looking for one thing that matches the paramaters set between those two characters.

### Quantifiers
Thes components determine the numner of a given character that the regex is looking for. In this example, the + quantifier is used. The + is looking for at least one of the preceding characters to be present. For example, the first + in the example is making sure there is at least one a-z letter, 0-9 digit, _ \ . or - for it to match. those requirements are shown between the [] just before the +.
{} fill a similar role but can be filled with a first and second digit to signify a min/max, { n, } for at least a given number, or { n } for exactly a given number.

### Grouping Constructs
() is a grouping construct used to isolate different bits of the regex, similar to how PEMDAS works in a math setting. In this example, the first set requires a letter, number, or one of the previously listed special characters. The second () contains code for looking for digits

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
