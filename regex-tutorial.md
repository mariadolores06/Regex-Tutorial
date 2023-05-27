## Regex Tutorial: Matching a URL

This following gist gives a breakdown of the regular expression, regex, used for matching a URL. 

## Summary

The regex below can be used to validate a URL and has been broken down by its components. Each section describes the symbol, where it is found in the regex, and a description. 

<code>/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/<code>


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

The two characters used as anchors are <code>^<code>, which is at the beginning and <code>$<code>, found at the end. 
Found in the regex:
/<code>^<code>(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?<code>$<code>/

They show where the text starts and ends in the expression. We are asking the search function to match exactly what is included between them (what it begins AND ends with).

### Quantifiers

<code>/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/<code>


### Grouping Constructs

<code>/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/<code>


### Bracket Expressions

<code>/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/<code>


### Character Classes

<code>/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/<code>


### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
