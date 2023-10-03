# Regex Turorial

Regular Expressions (regex) provide us with a powerful tool for pattern matching and searching within text. Mastering regex can streamline many tasks, from data validation to content extraction. This tutorial will delve deep into one specific regex pattern: the pattern for matching an email address. Through this, we aim to provide clarity on regex components and their applications.

## Summary

We will be diving into the regex pattern for matching standard email addresses. The general structure of an email is localpart@domain.com. Here's a simple regex that matches an email:

^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$

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

### Regex Components

## Anchors

In our regex, ^ and $ are anchors representing the start and end of a line, respectively. They ensure the entire string is an email.

Example: ^ ensures "test@domain.com" is matched but not "hello test@domain.com".

## Quantifiers

The + symbol allows one or more occurrences of the preceding character or group.

Example: a+ would match 'a', 'aa', 'aaa', etc.

## OR Operator

We did not utilize the OR operator in this specific regex.

## Character Classes

[a-zA-Z0-9._%+-] matches any single character in the set. This set includes upper and lowercase letters, numbers, and some special characters commonly found in email addresses.

Example: "test.email+filter@domain.com" is valid.

## Flags

We did not specify flags in this regex, but they could be used to modify the search behavior, like making it case insensitive.

## Grouping and Capturing

We did not utilize groups in this regex, but they can be used to group portions of the pattern and capture content.

## Bracket Expressions

[a-zA-Z] matches any single alphabetic character, either lowercase or uppercase.

## Greedy and Lazy Match

The + quantifier is greedy by default, meaning it matches as much as possible. We didn't specify lazy matching in this regex.

## Boundaries

The @ symbol ensures there is only one @ character separating the local part from the domain of the email.

Example: "test@domain.com" is valid but "test@@domain.com" is not.

## Back-references

We did not utilize back-references in this regex.

## Look-ahead and Look-behind

We did not utilize look-aheads or look-behinds in this regex. They can be used to assert what is or isn't directly before or after the current position in the match.

## Author
Juan Francisco Grillo
[JuanFranciscoGrillo]