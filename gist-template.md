# RegExTutorial

For this assignment, I will be breaking down the regular expression for matching a Hex Value. 


## Summary


The following regular expression: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ is used for matching hexadecimal color codes in HTML and CSS. In this tutorial, I will be breaking down the regular expression into its components and explaining what each component does.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

The first anchor in the regular expression is the caret (^). The caret is used to match the beginning of a string. In this case, the caret is used to match the beginning of the string that is being tested.

The second anchor in the regular expression is the dollar sign ($). The dollar sign is used to match the end of a string. In this case, the dollar sign is used to match the end of the string that is being tested.


### Quantifiers

The first quantifier in the regular expression is the question mark (?). The question mark is used to match the preceding character zero or one time. In this case, the question mark is used to match the preceding character (#) zero or one time. For example, the regular expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ would match the strings "#000000", "000000", because they all represent valid hexadecimal color codes. To summarize, the hash symbol (#) is optional in this regular expression because of the question mark (?).

The second quantifier in the regular expression is the curly braces ({}). The curly braces are used to match the preceding character a specified number of times. In this case, the curly braces are used to match the preceding character ([a-f0-9]) six times or three times. For example, this regular expression would match strings like '#3e1a8f' or 'a1b' because they represent valid hexadecimal color codes. To summarize, this regular expression is looking for a string that matches one of two patters: either a sequence of exactly 6 or 3 hexadecimal digits, where each character is a hexadecimal digit or a number between 0-9.


### OR Operator

The OR operator, also known alternation, in the regular expression is the pipe (|). The pipe is used to match either the character on the left or the character on the right. In this case, the pipe is used to match either the character on the left ([a-f0-9]{6}) or the character on the right ([a-f0-9]{3}). So, the regular expression matches strings that may or may not contain a hash symbol followed by a sequence of exactly 6 hexadecimal characters or a sequence of exactly 3 hexadecimal characters.



### Character Classes

The only character class noted within this regular expression is: a-f0-9. After conducting some research, I have found that character classes enclosed within square brackets [], and they specify a range of characters that the REGEX engine can match. In this particular regular expression, the character class matches any character that is a lower case letter between a through f as well as any digit from 0 through 9. 












### Grouping and Capturing

The first group in the regular expression is the parentheses (()). The parentheses are used to group together the characters inside of the parentheses. In this case, the parentheses are used to group together the characters inside of the parentheses ([a-f0-9]{6}|[a-f0-9]{3}).

The second group in the regular expression is the square brackets ([]). The square brackets are used to match any character that is inside of the square brackets. In this case, the square brackets are used to match any character that is inside of the square brackets ([a-f0-9]).

The third group in the regular expression is the curly braces ({}). The curly braces are used to match the preceding character a specified number of times. In this case, the curly braces are used to match the preceding character ([a-f0-9]) six times or three times.



### Bracket Expressions

The first bracket expression in the regular expression is the square brackets ([]). The square brackets are used to match any character that is inside of the square brackets. In this case, the square brackets are used to match any character that is inside of the square brackets ([a-f0-9]).

The second bracket expression in the regular expression is the curly braces ({}). The curly braces are used to match the preceding character a specified number of times. In this case, the curly braces are used to match the preceding character ([a-f0-9]) six times or three times.



### Greedy and Lazy Match

The first greedy match in the regular expression is the asterisk (*). The asterisk is used to match the preceding character zero or more times. In this case, the asterisk is used to match the preceding character ([a-f0-9]) zero or more times.

The second greedy match in the regular expression is the plus sign (+). The plus sign is used to match the preceding character one or more times. In this case, the plus sign is used to match the preceding character ([a-f0-9]) one or more times.

The third greedy match in the regular expression is the question mark (?). The question mark is used to match the preceding character zero or one times. In this case, the question mark is used to match the preceding character ([a-f0-9]) zero or one times.

The fourth greedy match in the regular expression is the curly braces ({}). The curly braces are used to match the preceding character a specified number of times. In this case, the curly braces are used to match the preceding character ([a-f0-9]) six times or three times.


## Author

GitHub Username: Kriskris9
GitHub URL: https://github.com/Kriskris9

