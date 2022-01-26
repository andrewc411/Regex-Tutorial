# Regex Tutorial: Matching an Email

Regular expressions, also known as regex, are ways to search through a string of text. They are a sequence of characters that defines a search pattern and can be used to validate input. For this tutorial, we will be looking at the regex for matching an email. This regex is typically used with technologies like MongoDB and Node's Inquirer to validate emails.

## Summary
```/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/```<br>
This is the regular expression used to ensure that the email matches. This tutorial will be going over the different characters that are standard to a regex and other components that allow for this specific regex to be succesful.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)

## Regex Components
By putting a '/' at the beginning and end of a regex you make it a literal.

### Anchors
The characters ^ and $ are both considered to be anchors. The ^ is used at the start of the regex and signifies a string that begins with the characters that follow it. The $ is used at the end of the regex and signifies a string that ends with the characters that precede it.
 
### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)