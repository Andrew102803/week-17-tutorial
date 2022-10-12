# Regex URL step by step

Regex Tutorial uRL Matching

A regular expression, or regex is a very wide term that encompoeeses many things. this regex is a bunch of characters that can be used to assure accruate and valid user input for a url. This tutorial will break it down for a matching url

## Summary

The url displayed here will be able to validate a url and has been broken down by its compoinents (a anchor or grouping contact etc) each section past this will describe each one 

Regex for url `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)

## Regex Components
The componets listed below
### Anchors
a anchor is very simple ^ Asserts the position in the start of the string. and is very simply the beggiing 
Code in Regex: ``/^(h``
A dollar sign $ meanwhile Asserts the position at the end of the string or before the end of the string's line terminator if needed
code in regex: ``/?$/``
### Quantifiers
This section is the longest so i will be firm and to the point here 
?	Matches the previous token between 0 and 1 times, as many times as possible, giving back as needed.
regex:``(https?:\/\/)? matches the characters https : // literally``
(*)	Matches the prevoius token between 0 and unlimited times, as many times as possible, giving back as needed.
regex: ``([\/\w \.-]*)*``
(+)	Matches the previous token between 1 and unlimited times, as many times as possible, giving back as needed.
regex; ``([\da-z\.-]+)``
{2,6}	Matches the previous token between 2 and 6 times, as many times as possible, giving back as needed.
regex; ``([a-z\.]{2,6})``
### Grouping Constructs 
grouping contacts are short and simple they simply group everything inclosed within
regex:``(https?:\/\/)?``
### Bracket Expressions
braket expreesioons are used for placing charcters in the url
[a-z]	Matches a single character in the range between well A and Z as would be expected
regex: ``[a-z\.] matches a single character in the range between a & z with a character. OR [\da-z\.-] matches a single character in the range between a & z, before one digit equivalent to [0-9] & the characters . & -``
regex: ``[ \/ \w \.-]	Matching a single character present in the list to the right:``
regex: ``\/ = matches the character /``
\w = matches any word character equivalent to [a-zA-Z0-9_] \. = matches the character . = matches the character -
### Character Classes
these do the same as brackets but with digits 
\d	Matches a single character that is a digit.
regex: ``([\da-z\.-]+)``
\w	Matches any word character. Alphanumeric charatcer plus underscore.
regex: ``[\/\w \.-]``
### Character Escapes
Much like the last few charcter escapes ecist to match digits or words
\d	Matches a single character that is a digit.
regex: ``([\da-z\.-]+)``
\w	Matches any word character. Alphanumeric charatcer plus underscore.
regex: ``[\/\w \.-]``
## Author
Andrew Miller arm102803@gmail.com 
https://github.com/Andrew102803
