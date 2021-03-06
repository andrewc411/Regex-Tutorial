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
Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. Ordinarily, quantifiers are greedy; they cause the regular expression engine to match as many occurrences of particular patterns as possible. Appending ? to a quantifier makes it lazy; it causes the regular expression engine to match as few occurrences as possible. They appear in curly brackets as {2,6}. 2 would be the minimum number and 6 the maximum number that the regex should look for. Another quantifier in this expression is the + which combines the parts of the email together.
### Grouping Constructs
The primary way you group a section of a regex is by using parentheses. Each section within parentheses is known as a subexpression. And the pairing of separate subexpressions in a regex is known as grouping constructs.
### Bracket Expressions
Anything inside brackets that represents a range of characters that we want to match are known as bracket expressions. They are also known as a positive character group, because they outline the characters we want to include. Bracket expressions can be turned into negative character roups by add a ^ to the beginning of the expression. In this case, all charcters "a" through "z", numbers "0" through "9", and the characters "_.-" are accepted. Using hyphens between the letter and the numbers signify the range of the letters and numbers.
### Character Classes 
When using \d for the matching email this character class will match one character from any numeral digit 0-9.
### Character Escapes
The back slash \ in a regex is a character escape, which signifies a charcter that is not to be taken literally. A period in a regex would match any character except the newline character (/n) but when matching an email "." it just means to look for a period.
## Author
Andrew Carroll is a software developer that is enrolled in Georgia Tech's Full Stack Web Dev Bootcamp. You can visit his GitHub profile here: https://github.com/andrewc411