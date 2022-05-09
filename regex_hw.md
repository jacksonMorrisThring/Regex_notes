# 📖 Using Regex to validate phone numbers [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project utilises the properties of regex functions to explain how phone numbers in a varitety of forms can be searched for and validated based on certain acceptance criteria. Regex functions are nearly universal in use accross programming languages, and even form core principles in languages like Pearl.

## Summary

\(?\(\+\d{2}\) ?\d{3}[-.)](\d{3})[-.]\d{3}

The above regex expression is the one I will use to make clear the principles of Regular expressions. Above is a regex statement used to validate Australian phone numbers. E.g. (+xx) at the beginning for area code, followed by 3 numbers, then a space (or - or .), then 3 numbers, then a space (or - or .), then, finally, 3 more numbers.

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

Each component can be subdivided into sections where the \ marks a new criteria. The first component starts with 
    \(
This tells the computer that the valid string should start with a bracket (. Then...
    \+
tells the computer that the valid string should next have a + sign. Then...
    \d{2}
tells the computer that the valid string should next have a 2 digits. Then...
    \)
tells the computer that the valid string should next have a closing bracket ). Together ( \(\+\d{2}\) ), this validates that the phone number should start with (+xy). By stringing statements like this together, regex allows the user to specify a find request based on non-specific critria (generalised  numbers, letters, or symbols).

### Anchors

No anchors are specifically used in this case, but anchors in general dont match particular characters but locations within strings of characters in which to look. E.g. ^ specifies to look at the beginning of the string, while $ specifies to look at the end of a string

### Quantifiers

Quanitifers are used to specify how many instances of one thing should be found. It saves you repeating a certain expression multiple times. E.g. instead of saying \d\d\d you could say \d{3}. Here, the {x} is the quanitifer, and this can be visibly seen above when specifying how many digits each part should contain.

## Author
Jackson Morris-Thring

Any additional questions? Reach me at jacksonmorristhring2000@gmail.com
View my github profile and previous projects at https://github.com/jacksonMorrisThring
