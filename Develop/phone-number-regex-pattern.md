# Regex Tutorial for Phone Numbers

Phone numbers come in various formats and can be challenging to extract or validate from a given text. Regular expressions (regex) are powerful tools for pattern matching and can be used to create a regex pattern that matches phone numbers. This tutorial will explore a common regex pattern for matching phone numbers, explaining its various components such as anchors, quantifiers, character classes, flags, grouping and capturing, bracket expressions, greedy and lazy match, boundaries, back-references, look-ahead, and look-behind.

## Summary

The regex pattern we will be explaining is:

```^(\+?\d{1,3}[-.])?\(?(\d{3})\)?[-.]?\d{3}[-.]?\d{4}$```

This pattern is designed to match phone numbers that may be in various formats, including those with or without country codes, area codes, and different delimiters such as hyphens, dots, or parentheses. It uses anchors, quantifiers, OR operators, character classes, flags, grouping and capturing, bracket expressions, greedy and lazy matching, boundaries, back-references, look-ahead, and look-behind to create a comprehensive phone number matching pattern.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

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

### Flags
The regex pattern does not use any flags, which are optional settings that modify the behavior of the regex engine, such as case sensitivity or global matching.

### Grouping and Capturing
The regex pattern uses parentheses ```()``` for grouping and capturing. This allows for capturing and extracting specific parts of the matched phone number. For example, ```(\d{3})``` captures the area code of the phone number for further processing.

### Bracket Expressions
The regex pattern uses bracket expressions such as ```[-.]``` to define a set of characters to be matched. It allows for specifying a range of characters or individual characters that are acceptable at a particular position in the pattern.

### Greedy and Lazy Match
The regex pattern uses greedy matching, which means it matches the longest possible string that satisfies the pattern. For example, ```\d{1,3}``` matches the longest possible sequence of one to three digits. However, the pattern can be modified to use lazy matching by adding a ```?``` after the quantifiers, such as ```\d{1,3}?```, which would make the matching as short as possible.

### Boundaries
The regex pattern does not use any boundary assertions, which are used to specify the position of a match in relation to word boundaries, line boundaries, or other specific boundaries in the text.

### Back-references
The regex pattern uses back-references, which refer to previously captured groups in the pattern. For example, ```(\d{3})``` captures the area code, and then ```\(?(\d{3})\)?``` uses a back-reference to refer to the captured area code again, allowing for matching phone numbers with or without parentheses around the area code.

### Look-ahead and Look-behind
The regex pattern does not use any look-ahead or look-behind assertions, which are used to specify conditions that must be met ahead or behind the current position in the text for a match to occur.

## Conclusion
In conclusion, the regex pattern provided is a comprehensive and flexible pattern for matching phone numbers in various formats. By understanding the different components of the pattern, including anchors, quantifiers, OR operators, character classes, flags, grouping and capturing, bracket expressions, greedy and lazy match, boundaries, back-references, look-ahead, and look-behind, you can effectively use this regex pattern for phone number validation or extraction tasks in your applications.

## Author
Created by Xavier Teo. For additional questions and information, please go to my GitHub profile at https://github.com/XvrTeo or reach out via email at xvrteo@gmail.com.
