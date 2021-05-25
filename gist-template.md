# Title (Regex Tutorial)
is a sequence of characters that specifies a search pattern. Usually such patterns are used by string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation. It is a technique developed in theoretical computer science and formal language theory.
This tutorial was created as an assignment for the University of Arizona's coding bootcamp. The purpose of this tutorial is to explain in detail how a specific regex functions by breaking down each part of the expression and describing what it does.

## summary
This tutorial will examine each character in the following regex in order to explain its overall function:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This regex matches an email. It can therefore be used to find email addresses within a string of text, verify that a user has entered a valid email address, etc.

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
Anchors belong to the family of regex tokens that don't match any characters, but that assert something about the string or the matching process. Anchors assert that the engine's current position in the string matches a well-determined location: for instance, the beginning of the string, or the end of a line.
The ^ and $ in the regex are Anchors, as seen in the beginning and end of the expression:
/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/
n our regex above, the beginning ^ and ending $ anchors indicate that the search must match characters defined by the piece of the expression located between the anchors: ([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6}) We will explain each of these components in their respective sections below.
