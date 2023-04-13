# Regex Tutorial for Phone Numbers

Phone numbers come in various formats and can be challenging to extract or validate from a given text. Regular expressions (regex) are powerful tools for pattern matching and can be used to create a regex pattern that matches phone numbers. This tutorial will explore a common regex pattern for matching phone numbers, explaining its various components such as anchors, quantifiers, character classes, grouping and capturing, bracket expressions, greedy and lazy match, and back-references.

## Summary

The regex pattern that will be covered in this tutorial is:

```^(\+?\d{1,3}[-.])?\(?(\d{3})\)?[-.]?\d{3}[-.]?\d{4}$```

This pattern is designed to match phone numbers that may be in various formats, including those with or without country codes, area codes, and different delimiters such as hyphens, dots, or parentheses. It uses anchors, quantifiers, character classes, grouping and capturing, bracket expressions, greedy and lazy match, and back-references to create a comprehensive phone number matching pattern.

### Breaking it down:

```^```: Represents the start of a line.

```(\+?\d{1,3}[-.])?```: Captures an optional country code, which can start with a "+" symbol, followed by 1 to 3 digits, and ending with a hyphen or period as a delimiter.

```\(?```: Optionally captures an opening parenthesis "(".

```(\d{3})```: Captures a group of three digits, representing the area code.

```\)?```: Optionally captures a closing parenthesis ")".

```[-.]?```: Optionally captures a hyphen or period as a delimiter.

```\d{3}```: Captures a group of three digits, representing the local exchange code.

```[-.]?```: Optionally captures a hyphen or period as a delimiter.

```\d{4}```: Captures a group of four digits, representing the subscriber number.

```$```: Represents the end of a line.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Back-references](#back-references)

## Regex Components
The regex pattern for matching phone numbers includes the following components:

### Anchors
The regex pattern starts with the ```^``` symbol, which is the caret anchor. It signifies the start of a line in the text, ensuring that the phone number pattern is matched at the beginning of the line.

### Quantifiers
The regex pattern uses various quantifiers such as ```{1,3}``` and ```{3}``` to specify the number of occurrences of digits to match. For example, ```\d{1,3}``` indicates matching one to three digits, and ```\d{3}``` indicates matching exactly three digits.

### OR Operator
The regex pattern uses the ```|``` symbol, which is the OR operator. It allows for multiple alternatives to be matched at a specific position in the pattern. For example, ```[-.]``` indicates matching either a hyphen or a dot.

### Character Classes
The regex pattern uses character classes such as ```\d``` to match any digit, and ```[-.]``` to match either a hyphen or a dot. Character classes are enclosed in square brackets ```[]``` and allow for matching a single character from a set of characters.

### Grouping and Capturing
The regex pattern uses parentheses ```()``` for grouping and capturing. This allows for capturing and extracting specific parts of the matched phone number. For example, ```(\d{3})``` captures the area code of the phone number for further processing.

### Bracket Expressions
The regex pattern uses bracket expressions such as ```[-.]``` to define a set of characters to be matched. It allows for specifying a range of characters or individual characters that are acceptable at a particular position in the pattern.

### Greedy and Lazy Match
The regex pattern uses greedy matching, which means it matches the longest possible string that satisfies the pattern. For example, ```\d{1,3}``` matches the longest possible sequence of one to three digits. However, the pattern can be modified to use lazy matching by adding a ```?``` after the quantifiers, such as ```\d{1,3}?```, which would make the matching as short as possible.

### Back-references
The regex pattern uses back-references, which refer to previously captured groups in the pattern. For example, ```(\d{3})``` captures the area code, and then ```\(?(\d{3})\)?``` uses a back-reference to refer to the captured area code again, allowing for matching phone numbers with or without parentheses around the area code.

## Conclusion
In conclusion, the regex pattern provided is a comprehensive and flexible pattern for matching phone numbers in various formats. By understanding the different components of the pattern, you can effectively use this regex pattern for phone number validation or extraction tasks in your applications.

## Author
Xavier Teo (https://github.com/XvrTeo)
