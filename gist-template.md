# Understanding the Anatomy of an Email Regex

Regular expressions, often called "regex", are like codes that help us find and match patterns in text. Imagine them as special search tools. In this guide, we'll look at a regex for spotting email addresses. By the end, you'll know how it works and how to read similar codes.

## Summary

Today, we're exploring a code that finds typical email addresses. The code is:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

We'll go through each part of this code and explain what it does.

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

- `^` : Matches the beginning of a line.
- `$` : Matches the end of a line.

In our regex, these anchors ensure that the pattern matches the entire string, from start to finish.

### Quantifiers

- `+` : Matches one or more of the preceding character or group.

In our regex, `+` ensures that we have one or more of the allowed characters before and after the `@` symbol, and also after the period (.) before the domain.

### OR Operator

Not used in this regex.

### Character Classes

- `\d` : Matches any digit (0-9).
- `.` : Matches any single character (in this case, it's escaped to match the literal period).

In the email regex, `[\da-z\.-]` will match any single digit, lowercase letter, period, or hyphen.

### Flags

No flags are used directly in this regex, but flags can modify how a regex behaves. For example, `i` for case insensitive.

### Grouping and Capturing

- `()` : Creates a capture group.

In our regex, there are three capturing groups:
1. Local part of the email (before the `@`).
2. Domain name (between `@` and `.`).
3. Top-level domain (after the `.`).

### Bracket Expressions

- `[]` : Matches any single character contained within the brackets.

Here, `[a-z0-9_\.-]` matches any lowercase letter, digit, underscore, period, or hyphen. Similarly, `[\da-z\.-]` matches digits, lowercase letters, period, or hyphen.

### Greedy and Lazy Match

Only greedy matching is used here, as there's no `?` following a quantifier.

### Boundaries

Not specifically used in this regex.

### Back-references

No back-references are used in this regex.

### Look-ahead and Look-behind

Not used in this regex.

## Author

JuanFranciscoGrillo 
[JuanFranciscoGrillo]
