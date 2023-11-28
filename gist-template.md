# Regex Tutorial - Matching a Hex Value

Developers write code, but they also write about code. Take a moment to search the web for tutorials about any of the subjects you’ve learned so far in this course. You’re likely to find thousands of tutorials written by developers of all skill levels, but especially by junior developers—like you!
Your Challenge this week is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. You'll use the template provided in the starter code to create your tutorial.

AS A web development student
I WANT a tutorial explaining a specific regex
SO THAT I can understand the search pattern the regex defines

## Summary

This regex will match a hex value. A hex value is a 6 digit combination of letters and numbers. The regex will also match a 3 digit combination of letters and numbers. The regex will match any character in the range of a-f or 0-9. The regex will match the pattern 0 or 1 times, which means it will match, or it will not match a superceding hex value. The regex will capture either 6 or 3 characters using the logical OR.

```/^#?([a-f0-9]{6}|[a-f0-9]{3})$/```

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
The matching a hex value regex can be split into two comoonents with the logical OR operator:

```^#?([a-f0-9]{6}```

and 

```[a-f0-9]{3})```

The first component will match a hex value with 6 characters, noted with the `{6}` quantifier. The `#?` quantifier means that the `#` character is optional. The bracket expression `[a-f0-9]` means that the regex will match any character in the range of a-f or 0-9.

The second component will match a hex value with 3 characters, noted with the `{3}` quantifier. The bracket expression `[a-f0-9]` means that the regex will match any character in the range of a-f or 0-9.


### Anchors
`^` and `$` are start and end of line anchors.

### Quantifiers
The quantifiers in the regex are `{6}` and `{3}`. This means that each side of the logical OR operator must have either 6 or 3 characters.
Another quantifier is the `#?`, which means on the left side of the regex, the `#` character is optional.

### OR Operator
The OR operator in the regex is `|`. This means that the regex will match either side of the operator.

### Character Classes
The character classes in the regex are `[a-f0-9]` and `[a-f0-9]`. This means that the regex will match any character in the range of a-f or 0-9.

### Flags
There are no flags in this regex.

### Grouping and Capturing
The grouping and capturing in the regex is `([a-f0-9]{6}|[a-f0-9]{3})`. This means that the regex will capture either 6 or 3 characters.

### Bracket Expressions
The bracket expressions in the regex are `[a-f0-9]` and `[a-f0-9]`. This means that the regex will match any character in the range of a-f or 0-9.

### Greedy and Lazy Match
The greedy match in the regex is `{6}` and `{3}`. This means that the regex will match either 6 or 3 characters. The lazy match in the regex is `?`. This means that the regex will match the pattern 0 or 1 times.

### Boundaries
Boundaries, indicated by `\b`, are not used in this regex.

### Back-references
Back-references, indicated by `\1`, are not used in this regex.

### Look-ahead and Look-behind
Look-ahead, indicated by `(?=...)` and `(?!...)`, is not used in this regex. Look-behind, indicated by `(?<=...)` and `(?<!...)`, is not used in this regex.

## Author
Weston Kostura

Github: https://github.com/westonkostura