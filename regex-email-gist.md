# Email Address Regex Gist

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
Thes components determine the numner of a given character that the regex is looking for. In this example, the + quantifier is used. The + is looking for at least one of the preceding characters to be present. For example, the first + in the example is making sure there is at least one a-z letter, 0-9 digit, _  . or - for it to match. those requirements are shown between the [] just before the +.
{} fill a similar role but can be filled with a first and second digit to signify a min/max, { n, } for at least a given number, or { n } for exactly a given number.

### Grouping Constructs
() is a grouping construct used to isolate different bits of the regex, similar to how PEMDAS works in a math setting. In this example, the first set requires a letter, number, or one of the previously listed special characters. The second () contains code for looking for digits, a-z letters, or -
The third () does the same thing, but only in a length of 2-6

### Bracket Expressions
Simply put, [] is looking for any instance of the instructions put inside of it. similar to the () but it caries its own effect.
### Character Classes
. looks for any character. `\.` looks just for the period itself. Also \d looks for any number. similar to [0-9]
### The OR Operator
not present in this example, the | is the OR operator, it searches for the preceding or following characters.
### Flags
not present in this example, but flags are placed after the / wrapper and put certain limits on the regex. g is global search, it will try the match the regex against all characters in a string. i is case-insensitive-search, it will ignore the difference between upper and lowercase letters when running the regex. m is multi-line-search, multiple lines in a regex input will be treated as having multiple lines.
### Character Escapes
\ is an escape character that exempts the following character from being interpreted literally. It can be used for various special functions. An example being \d being used as [0-9] rather than just \ and d.
## Author
Jarrett Stavey is a full-stack web developer, and he hopes you found this regex interesting and informative! You can visit my GitHub profile at https://github.com/JStavey13 
email me with any questions or comments at jstavey13@icloud.com

