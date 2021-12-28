# Email Regex Tutorial

A simple, straightforward breakdown of an email regex. Through this explanation, you'll be able to understand each individual component that comprises this email regex. Components included here are [anchors](#anchors), [quantifiers](#quantifiers), [bracket expressions](#bracket-expressions), [character classes](#character-classes), and [character escapes](#character-escapes).

This is a great website to use for reference and to test out your test strings:
[regex101.com](https://regex101.com/)

## Summary

In this tutorial, we'll be going over this email regex, as shown below:

`^([a-zA-Z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)

## Regex Components


### Anchors

The anchor `^` signifies the start of the string for this expression. While the anchor `$` signifies the end of it.


### Quantifiers

The `+` quantifiers that follow the `]` match the tokens provided in the `[]` an unlimited number of times.
Also included in this regex are the `{}`, which for us, contain a `2` and a `6`. This means that they will match the previous token between 2 and 6 times. A term that is used to describe quantifiers is `greedy`, meaning they will match as many times as possible. A quantifier can be made `lazy` by adding the `?` symbol after closing `}`, so that it will match as few times as possible.


### Bracket Expressions

The contents inside these `[]` consist of a range of expressions that we want our potential email to match. Included in our expression are:
- `a-z` (all lowercase letters)
- `A-Z` (all uppercase letters)
- `0-9` (all numbers from 0-9)

Also included in our brackets are the `_` and `-`. These will just match literally.


### Character Classes

The character class we are using here is the `\d`. This matches any number, the same as `[0-9]` would.


### Character Escapes

The `\` here is a character escape. It prevents the period that follows it from being read as a character class, and instead tells the expression to look for a period character.


## Author

Gabrielle Humkey, full-stack developer in training.

Github: [github.com/humkeyg](https://github.com/humkeyg)
