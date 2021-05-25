# Title (Regex Tutorial)
is a sequence of characters that specifies a search pattern. Usually such patterns are used by string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation. It is a technique developed in theoretical computer science and formal language theory.
This tutorial was created as an assignment for the University of Arizona's coding bootcamp. The purpose of this tutorial is to explain in detail how a specific regex functions by breaking down each part of the expression and describing what it does.

## summary
This tutorial will examine each character in the following regex in order to explain its overall function:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This regex matches an email. It can therefore be used to find email addresses within a string of text, verify that a user has entered a valid email address, etc.

