# Regex Tutorial:

In general we emphasize more on writing down the codes but it is equally important what they are and their's functionality. This tutorial explains how a specific regular expression, or regex, functions.

## Summary

A **regualr expression**, which is shorty called **regex**, is a way of explaining the certain type of formats in a string data. Regex are mostly used to validate for prompts input by users. Basically, it is apply to search, match, and replace the specific orders of string of character or sets of characters. 
 
For example, the following regular expression  make sure valid URL address:

`/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

In the given regex, each symbol has their own individual functionality to match the corrects inputs character and orders while user enters any URL address


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

Anchors are used at the begaining and ending of the expression.
``` 
^ symbol is anchor that matches the beginning of input.
$ symbol is  anchor that matches the ending of input.
```


### Quantifiers
Quantifiers are symbols that have a special meaning in a regular expression which determine how many times a certain character or group of characters should be exist to have the match. 
```
Eaxample

/ba+g/ will match the strings 'bag', 'baag', baaag', baaaag', and so on.
 The expression will look for b followed by a, one or more tahn one times and then finally g. 
 So, the searching will end at g.

```

### Grouping Constructs

Grouping constructs are used to make sure more than one parts of a string in order to determine that different sections satisfied different requirements. Generally, grouping a section of a regex is done by using (`()`) parenthesis.
```md
/^[a-zA-Z0-9.!#$%&’*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/
as
/^...........(................).$/
```


### Bracket Expressions
This expression is based on the characters that are enclosed by a bracket []. 
It is applied to match the characters inside the brackets. 
Examples of Brackets Expression are as follows;
```
[^] - It applied to all the string excepts those are within brackets.
[]% - IT applied to all the string within  a brackets before %
[] - It applied to each string within the brackets. 
```

### Character Classes
It simply match a characters from a specific set of characters.
```
[A-Z] make sure alphabetics charaters are A to Z
. matches to all the character
\w make sure it is word
\d make sure character that is a digit
```
### The OR Operator

It is used in those scenario where the selection result has probability on both side of expression seprated by |.
For examples
 ```
 [a-z{1}]|[A-Z{2}] 
 In this example the answer would be 1 or 2.
 ```



### Flags
Flags are the expressions denoted by a single alphabetical character, and applied to change the search pattern.

```
u (Unicode) make sure the expression target the individual characters as  code points instead of code units. So it it can match 32-bit characters as well.
i - (Ignore casing) which will make the entire expression case sensitive
g - (Gloabal) make sure the expression search for all occurences
m - (Multiline) used to create the beginning ^ and ending $ anchors to match the start and end of a line instead of the whole string

Y(Sticky) Makes the expression start its searching from the index indicated in its last index property

```



### Character Escapes

It is denoted to \ backslash. In regex it is used to escape the next character which let the developer include reserved character like []{}+*$^?|. as matching characters.

## Author

Rajesh Gautam is the students at John Hopkins University cooding boot camp who is looking forward to explore the carrier in coding world in near future. 

* [GitHub Profile](https://github.com/Rajesh295-dev)
