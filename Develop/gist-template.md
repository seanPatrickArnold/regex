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

"Anchors belong to the family of regex tokens that don't match any characters, but that assert something about the string or the matching process. Anchors assert that the engine's current position in the string matches a well-determined location: for instance, the beginning of the string, or the end of a line." - https://www.rexegg.com/regex-anchors.html 10/10/2021

Example: "/^A/" matches any string that begins with 'A' such that for the string 'Apple' the regex expression would retrun true.

### Quantifiers

"Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found." - https://docs.microsoft.com/en-us/dotnet/standard/base-types/quantifiers-in-regular-expressions 10/10/2021

Example: "/b7\*/b" would match "77" and "7" but not "78".

### OR Operator

"Alternatives match one of a choice of regular expressions: if you put the character(s) representing the alternation operator between any two regular expressions a and b, the result matches the union of the strings that a and b match. For example, supposing that `|' is the alternation operator, then `foo|bar|quux' would match any of `foo', `bar' or `quux'." - http://web.mit.edu/gnu/doc/html/regex_3.html 10/10/21

### Character Classes

"With a 'character class', also called 'character set', you can tell the regex engine to match only one out of several characters. Simply place the characters you want to match between square brackets. If you want to match an a or an e, use [ae]. You could use this in gr[ae]y to match either gray or grey." - https://www.regular-expressions.info/charclass.html 10/10/2021

### Flags

"Regular expressions have optional flags that allow for functionality like global searching and case-insensitive searching. These flags can be used separately or together in any order, and are included as part of the regular expression." - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions 10/10/21

Example "/FoxAndTheHound/i" would match "foxandthehound" or FOXANDTHEHOUND".

### Grouping and Capturing

"Groups and ranges indicate groups and ranges of expression characters." - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Groups_and_Ranges 10/10/21

Example: "/[a-g]/" matches the all of the characters in "baggage" but only "ca" in "cat".

### Bracket Expressions

"A bracket expression is a list of characters enclosed by ‘[’ and ‘]’. It matches any single character in that list. If the first character of the list is the caret ‘^’, then it matches any character not in the list, and it is unspecified whether it matches an encoding error. For example, the regular expression ‘[0123456789]’ matches any single digit, whereas ‘[^()]’ matches any single character that is not an opening or closing parenthesis, and might or might not match an encoding error." - https://www.gnu.org/software/grep/manual/html_node/Character-Classes-and-Bracket-Expressions.html 10/10/21

### Greedy and Lazy Match

Greedy match denoted by by .+ surrounded by the wrapping characters will isolate all characters between the first instance of the character to the left of the .+ expression and the last instance of the character to the right of the .+ expression contained within a single line. Lazy match will find every set of characters contained between an instance of the the character to the left of the .+? expression and the character to the right of the .+? expression by isolating the next instance instead of searching backwards from the end of the string or line[https://javascript.info/regexp-greedy-and-lazy, 10/10/21.]

Example: ".+" will isolate 'cat' and 'dog' in "there is a 'cat' and 'dog' around the corner" and '.+?' will isolate 'cat' separately from 'dog' in the same string.

### Boundaries

"The metacharacter \b is an anchor like the caret and the dollar sign. It matches at a position that is called a “word boundary”. This match is zero-length." - https://www.regular-expressions.info/wordboundaries.html 10/10/21

Example: /bcat/b matches "cat" in "the cat scats" but not the characters "cat" contained within the word "scat".

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
