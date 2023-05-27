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

Quantifiers are used to define the number of times a given expression may be identified. 

<code>?<code> matches the token 0-1 times.
    This character is optional, but the regex will still look to see if it's present. 
<code>(https?:\/\/)?<code> matches the characters: https://

<code>*<code> matches the token between 0 and unlimited times. 
    This part allows for any combination of characters within the [ ] and it can be repeated any number of times. This will be any text that comes after the top level domain.
Found in the regex: 
<code>([\/\w \.-]*)*<code>

<code>+<code> matches the token between 1 and unlimited times.
    This part of the regex is looking for any of the charcters specified in [ ] and it is required to match at least one of those characters. 
Found in the regex: <code>([\da-z\.-]+)<code>

<code>{2,6}<code> matches the token betwen 2 and 6 times. 
    The numbers inside {} will determine what the regex will match. If there is only one number, then the regex will only match charcters that specified number of times. This portion would translate to the top level domain part of the URL. (.com, .edu, .org, etc.) Most top level domains are between two and six characters long.
Found in the regex: <code>([a-z\.]{2,6})<code>


### Grouping Constructs
    Grouping in a regex is done by simply wrapping the portion of the regex that you'd like to group in parenthesis. Grouping a part of the regex allows you to apply a quantifier to the group.
Found in the regex: <code>/^(https?:\/\/)?<code>

### Bracket Expressions / OR Operator
    A bracket expression is a list of characters enclosed by two square brackets. 
Found in the regex: <code>[\da-z\.-]<code> 
    This expression matches for any digits <code>\d<code> OR any characters between a and z <code>a-z<code> OR any '.'<code>\.<code> OR any '-' <code>-<code>. 

### Character Classes

    The main charcater classes in this regex include: <code>\d<code> which looks for any digit and <code>\w<code> which looks for any alphanumeric character. 
Found in the regex: <code>[\da-z\.-]<code> <code>[\/\w \.-]<code>

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
