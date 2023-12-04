## REGEX URL Gist

Regex is similar to searching or matching code to the characters. Usually, there would be more characters used to match one character at a time. Characters used would not represent one character but also other characters that will match the string of characters. The reason for this tutorial is to get a better understanding of what REGEX is and useful it can be in any programming languages. Some string of REGEX characters can result or be created to create other strings of characters. This is what makes a string of REGEX useful in selecting certain texts or strings of characters. 

## Summary

The chosen regex that I will be covering is matching a URL which is: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`. The code contains a variety of characters which includes symbols such as `/`, `^`, \, `*`, `.`, `?`, `$`, `[]`, `{}`, and `+`. Throughout the whole gist, each characters will be explained in details.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Author](#author)

## Regex Components

A REGEX components includes a `/` at the beginning and another `/`. It also includes a `^` and a `$` at the end to sigify that the first string have to include the parantheses after the `^` symbol.

### Anchors

The anchor characters includes two symbols which are: `^` and `$`. The `^` symbol is used to begin a set of strings or alphabtic character capitalized. The `$` is used to end the pattern or the `^` character. 

### Quantifiers

Quantifiers characters includes matching the pattern a number of times. Each symbol indicates such characters for that pattern. `*` would be where the pattern matches zero or more times. `+` would match the pattern one more times. `?` would match the pattern zero or one more time. `{}` would match the pattern an amount. `{1}` would be where the pattern matches one time. `{1,}` would be where the pattern matches at least one time. `{1, 3}` would be where the pattern would match one to three times. `{1, 10}` would be where the pattern matches one to ten more times.

### Grouping Constructs

Grouping constructs are a string of characters which will have the same character in the same postion. An example would be `(sun):(moon)` which means the string "sun:moon" would be the string to match this grouping construct.

### Bracket Expressions

Bracket Expression are used to choose one of the characters within the brackets. For example, the `[a-z]` will be an indicator of any lowercase letters. a, b, c, d, up to z can be the letter to be used. If we get `[0-9]`, this would mean that we get any number which is also similar to the `\d` character. In a common bracket which is used to make strings would be `[a-zA-Z0-9_-]`.

### Character Classes

The character classes is a bunch of character selectors in two uses of characters or less. Some character classes used are `.` which would match any character except the new line character. The `\d` string would match any one digit integer which is also similar to the `[0-9]` string. The `\w` would match any letter including uppercase and lowercase letters. It also includes one digit integer and also the `_` character as well. `[A-Za-z\d_]` would be similar to `\w`. `\s` matches a single space character or tabs and line breaks.

### The OR Operator

The `|` is a character used within the parantheses to choose one of a character which is different from the square bracket. Here is an example: `(1|2|3|4|5|6|7|8|9|0)`. This also match the string: `(0-9)` or also `\d`. If we 

### Flags

Flags are where the string will be searched for in a file. The character `g` is used to search the string globally. The character `d` is used to generate indices for substirng matches. `i` is used to search with case-insensitivity. 

### Character Escapes

The `\` is a character used before a special character to literally mean that character. An example in this case would be `\/` which would mean the `/` character and not `\/`. 

## URL Throughly Explained

`/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

1. `/` is used to begin the REGEX string
2. `^` is used to capitalized the string as a URL
3. `(https?:\/\/)?` matches https with the `:` which can matches 0 or more time. `https:\\` would work or `\\` would also work. The `?` would make the `https:\\` and `\\` match zero or one time.
4. `([\da-z\.-]+)\.` matches with a possiblity of having nothing or one digit or one lowercase letter or `.` or `-` character one or more times. That string would always have a `.` after the string.
5.`([a-z\.]{2,6})` would make the string that has at least 2 or 6 letters or `.` in that string. An example would `kdm.`
6. `([\/\w\.-]*)*` would includes a `\` or a uppercase, lowercase, one digit number, or `_`, `.`, `-` which would be match zero or more times and the whole string zero or more times. 
7. `\/?$/` would make the `/` character be match zero or one time. `$` would make the end of the anchor tag.

## Sources

1. https://www3.ntu.edu.sg/home/ehchua/programming/howto/Regexe.html#zz-1.
2. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions

## Author

Author: Jason Yang

GitHub Profile: https://github.com/Jasony95
