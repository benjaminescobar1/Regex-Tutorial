# Regex Tutorial- Match an Email

A regex, also known as regular expression, are text-based patterns encoded to search for specific patterns in other strings. They are extremely helpful when seeking to locate a sequence of characters that follow a particular pattern. A common usage would be to identify is a user has entered correct inputs into a form. 

## Summary

This tutorial is going to explain using regex to match emails using the following expressions "/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/".This regular expression ensures that the provided string follows the format of an email address.

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
The two main anchors used in this regex are ‘^’ and ‘$’. The anchor ‘^’ is used to start the string. The anchor ‘$’ is used to end the string.

### Quantifiers
In this regular expression, quantifiers play a significant role. The “+” operator connects the user's email name, the email service, and the ".com" portion. Additionally, there is another quantifier, {2,6}, which extends the flexibility by permitting a character set of [a-z.] to match a range of 2 to 6 characters.

### Grouping Constructs
Grouping and capturing are accomplished using parentheses (). Anything enclosed within a set of parentheses is considered a single group, allowing all the elements inside to be treated as a unified unit.

### Bracket Expressions
bracket expressions which are represented by three segments in our code: [a-z0-9_.-], [\da-z.-], and [a-z.]. A bracket expression denotes a single character, and this character can be any of the options specified within the brackets. For example, in [a-z0-9_.-], a character will be a match if it falls within the range of lowercase letters from 'a' to 'z', any digit from '0' to '9', or a period or hyphen.

### Character Classes
Regular expressions indeed employ special character classes to match specific types of characters. In our expression, "\d" is utilized to match any digit character. The backslash is essential here to distinguish the digit class from a simple lowercase "d."

### The OR Operator
N/A

### Flags
N/A

### Character Escapes
Character escapes are used to match specific characters within the regular expression. In this regex:

\_: The backslash \ before the underscore _ is used to escape the underscore, treating it as a literal character to match.

\., \-, and \/: Similarly, the backslashes before the period . , hyphen -, and forward slash / are used to escape these characters, so they are treated as literal characters to match.

\\d: The sequence \\d is used to match any digit character (0-9). The double backslash \\ is required because the single backslash is used as an escape character in regular expressions, and using \\ escapes the escape character itself.

Character escapes are crucial when you want to match characters that have special meanings in regular expressions as literal characters, rather than as part of the regular expression syntax.

## Benjamin Escobar

Benjamin Escobar is a fullstack web development student residing in the Bay Area. You can find more of his projects at https://github.com/benjaminescobar1.
