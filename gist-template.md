# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

An anchor is a piece of text which marks the beginning and/or the end of a hypertext link. The text between the opening tag and the closing tag is either the start or destination (or both) of a link.

### Quantifiers

Quantifiers indicate numbers of characters or expressions to match.
\*, +, ?, x{n}, x{n,}, x{n,m}

### OR Operator

### Character Classes

Character classes distinguish kinds of characters such as, for example, distinguishing between letters and digits.
Example: \, ., \cX, \d, \D, \f, \n, \r, \s, \S, \t, \v, \w, \W, \0, \xhh, \uhhhh, \uhhhhh, [\b]

### Flags

The flags property returns a string consisting of the flags of the current regular expression object.
Examples:
d: Generate indices for substring matches
g: Global search.
i: Case-insensitive search.
m: Multi-line search
s: Allows . to match newline characters.
u: "unicade"; treat a pattern as a sequence of unicode code points.
y: Perform a "sticky" search that matches starting at the current position in the target string.

### Grouping and Capturing

### Bracket Expressions

Bracketss indicate a set of characters to match. Any individual character between the brackets will match, and you can also use a hyphen to define a set.
Example: 'elephant'.match(/[abcd]/) // -> matches 'a'

### Greedy and Lazy Match

The quantifiers (\* + {}) are greedy operators, so they expand the match as far as they can through the provided text.
In order to catch only the div tag we can use a ? to make it lazy

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
