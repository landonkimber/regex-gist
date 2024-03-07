# Regex Guide

## Summary

This is a brief guide explaining regex, regular expressions. Regex allows you to search for and extract specific patterns of characters within strings. By using a combination of characters, quantifiers, and special symbols, regex enables precise and flexible matching in various programming languages and text processing applications. After reading this guide, be sure to check out https://regexr.com/ to see regex in action.

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

Anchors in regex specify the positions in the text where the pattern should match. 

-"^", caret key. The caret key asserts the start of a pattern.

-"$", dollar sign. The dollar sign asserts the end of a pattern

### Quantifiers

Quantifiers in regex allow you to specify how many times a character, group, or character class should match the input string.

-"\*", astrisk. Matches zero or more occurrences.

-"+", plus-sign. The plus sign matches one or more occurences.

-"?", question mark. The question mark matches zero or one occurrence of an element.

-"{n}". In this guide, n acts as a variable. In this case, "n" matches exactly n number of occurrences. Ex. {5} or {34}

-"{n,}". "n," matches at least n number of occurences.

-"{n,m}". The "n,m" will match anywhere beteween n and m number of occurences.

### OR Operator

The OR operator in regex, "|", will prompt to search for pattern A or pattern B.

### Character Classes

Character classes in regex allow you to match a single character from a set of characters. They can be defined by enclosing the characters within square brackets.

- "[ ]". Encloses a set of characters you want to match.

- "[a-z]". Matches any lowercase letter from 'a' to 'z'.

- "[A-Z]". Matches any uppercase letter from 'A' to 'Z'.

- "[0-9]". Matches any digit from '0' to '9'.

- "[^n]". Where n is a variable for any set of characters. Using the caret key, this character class matches any characters NOT listed within the square brackets.

- "\w", "\d", and "\s" refer to any word, digit, or whitespace.

- "\W", "\D", and "\S" refer to NOT any word, digit, or whitespace.

### Flags

Flags in regex are additional parameters that can be added to the regex pattern to modify its behavior.

-"i". Ignore case

-"g". Global. Matches all occurrences of a pattern.

-"m". Multiline. Allows ^ and $ to match the start and end of lines.

-"y". This expression will only match from its lastIndex position.

### Grouping and Capturing

Grouping in regex allows you to treat multiple characters as a single unit. We can use capturing groups to extract parts of a matched pattern.

-"()", parentheses. Creates a group and captures.

-"(?:)" This creates a group without capturing.

### Bracket Expressions

Bracket expressions allow you to match a single character from a specified set or range.

-"[]", brackets. Encloses a set of characters to match. Ex. [abc] matches "a", "b", or "c". 

-"[a-z]". Creates a range of characters to match.


### Greedy and Lazy Match

Greedy matches attempt to match as much of the string as possible while still allowing the entire pattern to match. A lazy match will match as little of the string as possible while still allowing the entire pattern to match

### Boundaries
Boundaries in regex specify positions in the text where certain conditions are met, such as the beginning or end of a word.

-"^", caret key. The caret key matches the beginning of a line.

-"$", dollar sign. The dollar matches the end of a line.

-"\b" & "\B", word boundary & non-word boundary.The capital and lowecase "b/B" are to match a word poundary position between a word character and non-word character.

### Back-references

Back-references allow you to refer back to previously captured groups within a regular expression pattern.

-"\n". Using the backslash, "\" and some number, we can reference to a previous group.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions in regular expressions specify conditions that must be met ahead of or behind the current position in the text, without consuming any characters.

-"(?=)". Positive look-ahead assertion - Checks if a pattern matches ahead.

-"(?!)". Negative look-ahead assertion - Checks if a pattern does not match ahead.

-"(?<=)". Positive look-behind assertion - Checks if a pattern matches behind.

-"(?<!)". Negative look-behind assertion - Checks if a pattern does not match behind.

## Author

Landon Kimber
landonkimber33@gmail.com
[landonkimber](https://github.com/landonkimber)
