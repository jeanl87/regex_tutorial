# Title: Regex Tutorial

This tutorial on regular expressions also known as regex.

## Summary

Regular expressions is a pattern that describes a set of strings that matches the pattern. Below is a breakdown of the different regex and examples to better understand the concept of these terms.

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

Examples: ^: anchor to match the beginning of the text (^. matches a in abc\ndef)
$: anchor to match the end of the text (.$ matches f in abc\ndef)

### Quantifiers

Quantifiers indicate numbers of characters or expressions to match.
Examples: \*, +, ?, x{n}, x{n,}, x{n,m}
\*: Match zero or more times
+: Match one or more times
?: MAtch zero or one times
{n}: Match exactly n times
{n,}: Match at least n times
{n,m}: Match from n to m times

### OR Operator

You can use the | operator (logical OR) to match characters ir expression of either the left or right of the | operator.

Example: the(t|T) will match either t or T from the input string.

### Character Classes

Character class is a set of chracters enclised within square brackets. It specifies the characters that will sucessfully match a single character from a given input string.

Examples:
[abc]: a, b, c (simple class)
[^abc]: Any character except a, b, or c (negation)
[a-zA-Z]: a through z, or A through Z, inclusive(range)
[a-d[m-p]]: a through d, or m through p: [a-dm-p] (union)
[a-z&&[def]]: d, e, or f (intersection)
[a-z&&[^bc]]: a through z, except for b and c: [ad-z] (subtraction)
[a-z&&[^m-p]]: a through z, and not m through p:[a-lq-z] (subtraction)

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

A group is part of a regex pattern enclosed in parenthese () metacharacter. We create a group by placing the regex pattern inside the set of parenthese (and).

Example: (cat) creates a single group containing the letters 'c','a','t'.

Capturing is a wat to treat multiple characters as a single unit. They are craeted by placing the characters to be grouped inside a set of parenthese.

Example: (dog) creates a single group containing the letters "d" "o" and "g".

### Bracket Expressions

Bracketss indicate a set of characters to match. Any individual character between the brackets will match, and you can also use a hyphen to define a set.
Example: 'elephant'.match(/[abcd]/) // -> matches 'a'

### Greedy and Lazy Match

The quantifiers (\* + {}) are greedy operators, so they expand the match as far as they can through the provided text.

Examples: (\*, +, {n}, {min,}, {0,max}, {min,max})

In order to catch only the div tag we can use a ? to make it lazy.

Examples: (??, \*?, +?, {n}?, {min,}?, {0,max}?, {min,max}?)

### Boundaries

The word boundaries:
Before the first character in a string if the first character is a word character.
After the last character in a string if the last character in a word character.
Between two characters in a string if one is a word character and the other is not.
Example: \b, \B

### Back-references

Back references are used to match the same text preivously matched by a capturing group.

Example: [0-9][-/ ][a-z][-/ ][0-9]

### Look-ahead and Look-behind

Lookahead asserts that what immediately follows the current position in an uppercase letter.

Lookbehind asserts that what immediately precedes the current position is a lowercase letter.

Examples:
(?!) - negative lookahead
(?=) - positive lookahead
(?<=) - positive lookbehind
(?<!) - negative lookbehind

## Author

Lisa Jean is a clinical research specialist. She is currently in the last section of fullstack web development bootcamp program for Coloumbia University.

Github link: https://github.com/jeanl87/regex_tutorial.git
