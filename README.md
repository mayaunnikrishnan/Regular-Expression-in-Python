# Regular Expression in Python

## Table of Contents
1. [Regular Expression Module in Python](#regular-expression-module-in-python)
2. [Meta Characters](#meta-characters)
3. [Sets](#sets)
4. [Special Sequences](#special-sequences)
5. [Regular Expression Functions](#regular-expression-functions)

## Regular Expression Module in Python:

- Python's regular expression module is called re.
- It provides functions for working with regular expressions in Python.
- Import the module using: import re

## Meta Characters:

Meta characters are special characters with unique meanings in regular expressions. They help define the structure and rules for pattern matching.

*Examples:*

-  `.`: Matches any single character except newline.
-  `^`: Matches the start of the string.
-  `$`: Matches the end of the string.
-  `*`: Matches zero or more occurrences of the preceding character.
-  `+`: Matches one or more occurrences of the preceding character.
-  `?`: Matches zero or one occurrence of the preceding character.
-  `|`: Matches either the expression before or after it.
-  `()`: Groups patterns together. Also used for capturing groups.
-  `{}`: Specifies the exact number of occurrences or a range of occurrences.
-  `[]`: Specifies a set of characters. Matches any single character within the brackets.
-  `\`: Escapes special characters, allowing them to be treated as literals.

## Sets 

Sets allow specifying a group of characters to match.

*Examples:*
-  `[abc]`: Matches any character a, b, or c.
-  `[0-5]`: Matches any digit from 0 to 5.
-  `[\d]`: Matches any digit (equivalent to [0-9]).
-  `[+]`: Matches the plus character.
-  `[a-c]`: Matches any character between a and c, inclusive.
-  `[a-z]`: Matches any lowercase alphabet character.
-  `[^arn]`: Matches any character except a, r, or n.
-  `[0-5][0-9]`: Matches any two-digit number from 00 to 59.

## Special Sequences:

Special sequences are shortcuts for commonly used patterns.
*Examples:*
-  `\A`: Matches the start of the string.
-  `\b`: Matches a word boundary.
-  `\B`: Matches where the string is not at a word boundary.
-  `\d`: Matches any digit character (equivalent to [0-9]).
-  `\D`: Matches any character that is not a digit (equivalent to [^0-9]).
-  `\s`: Matches any whitespace character.
-  `\S`: Matches any non-whitespace character.
-  `\w`: Matches any alphanumeric character (equivalent to [a-zA-Z0-9_]).
-  `\W`: Matches any non-alphanumeric character (equivalent to [^a-zA-Z0-9_]).
-  `\Z`: Matches the end of the string.
-  `\t`: Matches a tab character.
-  `\n`: Matches a newline character.
-  `\r`: Matches a carriage return character.
-  `\f`: Matches a form feed character.
-  `\v`: Matches a vertical tab character.
-  `{n:m}`: Matches at least n and at most m occurrences of the preceding character or group.
-  `(?:)`: Non-capturing group. Groups multiple tokens together without creating a capture group.

## Regular Expression Functions:

-  `re.compile(pattern)`: Compiles a regular expression pattern into a regex object.
-  `re.search(pattern, string)`: Searches for the first occurrence of a pattern in a string.
-  `re.match(pattern, string)`: Matches a pattern at the beginning of a string.
-  `re.findall(pattern, string)`: Finds all occurrences of a pattern in a string and returns them as a list.
-  `re.sub(pattern, replace, string)`: Replaces occurrences of a pattern in a string with another string.
-  `re.split(pattern, string)`: Splits a string based on a pattern and returns a list of substrings.
-  `re.finditer(pattern, string)`:Finds all occurrences of a pattern in a string and returns an iterator yielding match objects.
