# Regular Expressions

Here I am going to showcase to the best of my ability the current knowledge that I have when it comes to regular expressions and problem solving. The use of a REGEX (regular expression) is versatile and the expressions will contain a series of characters that define a pattern to be matched. This in simpler terms means to create a filter that will generalize the data in a more understandable way.

## Summary

The table of contents gives a good indiction of what will be explained in more detail in this tutorial. Giving some examples and explaining in plain english as well as possible. The goal of this tutorial is explain concepts that seem intimidating but instead are actually simple once you break them down, much is how almost all of coding is broken down.

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

The anchors in REGEX asser the current position in the string, often the beginning or end of the string. For example....

'123'.match(/^[0-9]+$/)

The start of the string must start with the ^ character. This is an anchor.

The end of the string must end with the $ character. This is also an anchor.

### Quantifiers

Quantifiers match a number of instances of a character, group, or character class in a string.

A good use of a quantifier is that it helps developers define how often an element occurs.

d{1,4} ; means d must occur at least once and at a maximum of four

### Grouping Constructs

Grouping constructs delineate the subexpressions of a regular expression and capture the substrings of an input string. You can use grouping constructs to do the following: Match a subexpression that is repeated in the input string.There are a variety of options that a grouping construct can be used for.

Match a subexpression that is repeated in the input string.

Retrieve individual subexpressions from the Match.Groups property and process them separately from the matched text as a whole.

### Bracket Expressions

A bracket expression (an expression enclosed in square brackets, "[]" ) is an RE that shall match a specific set of single characters, and may match a specific set of multi-character collating elements, based on the non-empty set of list expressions contained in the bracket expression.

### Character Classes

Character classes are enclosed in square brackets [ ] and can be used to match any character within the defined set.

Here are some examples of commonly used character classes:

[a-z]: matches any lowercase letter between a and z

[A-Z]: matches any uppercase letter between A and Z

[0-9]: matches any digit between 0 and 9

[a-zA-Z0-9]: matches any alphanumeric character

[^aeiou]: matches any character that is not a vowel (the ^ symbol within a character class means "not")

### The OR Operator

In regular expressions, the OR operator is denoted by the pipe symbol |. It allows you to specify alternative patterns that can match a given input.

Here are some examples of how to use the OR operator in regular expressions:

gr(e|a)y: matches either "grey" or "gray"

https?://: matches either "http://" or "https://"

(foo|bar)baz: matches either "foobaz" or "barbaz"

hello (world|there): matches either "hello world" or "hello there"

### Flags

Flags are optional modifiers that you can use to change the behavior of a regular expression. Flags are typically specified after the regular expression in the form of one or more letters.

`i`: the "ignore case" flag makes the regular expression case-insensitive. For example, the regular expression /hello/i will match "hello", "Hello", "HELLO", and so on.

`u`: the "unicode" flag enables full Unicode support in the regular expression. This includes support for Unicode characters in character classes and for Unicode-aware case-insensitivity.

### Character Escapes

Character escapes are denoted by a backslash (\) followed by a special code or character.

Here are some commonly used character escapes in regular expressions:

\d: matches any digit character (equivalent to [0-9]).

\w: matches any word character, including letters, digits, and underscores (equivalent to [a-zA-Z0-9_]).

## Author

This hopefully gives good insight to the knowledge that I am obtaining while attending the University Of Arizona Bootcamp through EdEx. I am excited to continue to learn something new each day and begin to master the tools that I am given making me a more efficient and more knowledgable coder.

https://github.com/colekasa
