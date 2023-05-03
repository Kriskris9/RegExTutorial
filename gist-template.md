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

The are are two anchors for this regular expression. The two anchors in this regular expression are the caret ```^``` and the dollar sign ```$```. In a regular expression the anchors are used to match the beginning and end of the string being tested. The caret matches the beginning of the string that is being tested while the dollar sign matches the end of the string being tested. 

### Quantifiers

There are two quantifiers in this regular expression. They are the question mark ```?``` and the curly braces ```{}```. The first quantifier in the regular expression is the question mark ```?```. The question mark in this regular expression makes the hash symbol ```#``` optional. So, you could have a hex value that starts with a hash symbol or you could have a hex value that does not start with a hash symbol. For example, the regular expression ```/^#?([a-f0-9]{6}|[a-f0-9]{3})$/``` would match the strings "#000000", "000000", because they all represent valid hexadecimal color codes. 

The second quantifier in the regular expression is the curly braces ```{}```. In this instance the curly braces make it so that it will match the pattern ```[a-f0-9]``` exactly six or three times. For example, this regular expression would match strings like '#3e1a8f' or 'a1b' because they both represent valid hexadecimal color codes and match the pattern. So to summarize this regular expression is checking to see if the string is following a pattern where it may or may not start with a hash symbol followed by a sequence of exactly 6 or 3 hexadecimal characters.

### OR Operator

The OR operator, also known as alternation, is represented with the pip character ```|```. In this regular expression, the OR operator will be used to match either the character on the left ```[a-f0-9]{6}``` or the character on the right ```[a-f0-9]{3}```. So, the regular expression will match any string that may or may not contain a hash symbol followed by a sequence of exactly 6 hexadecimal characters or a sequence of exactly 3 hexadecimal characters. 

### Character Classes

The only character class noted within this regular expression is: ```a-f0-9```. After conducting some research, I have found that character classes enclosed within square brackets [], and they specify a range of characters that the REGEX engine can match. In this particular regular expression, the character class matches any character that is a lower case letter between a through f as well as any digit from 0 through 9. 


### Bracket Expressions

The only bracket expression noted within this regular expression is: ```[a-f0-9]```. The square brackets in this regular expression define a character class, which is a set of characters that can match any single character at that position in the regular expression. The character class for this regular expression matches any single character that is either a lowercase letter between a through f or a digit between 0 and 9. 


### Grouping and Capturing

In this instance, the grouping would be the parenthesis ```([a-f0-9]{6}|[a-f0-9]{3})```. There is one main group within this regex, however, because of the or operator, it separates it into two small groups. So, you can either have a hex value that has 6 or 3 characters. 

### Greedy and Lazy Match

The greedy match, matches the longest string possibly, which in this case is ```[a-f0-9]{6}```. This string will be 6 characters long. 

While a lazy match is ```[a-f0-9]{3}```, which will be a 3 character long. The question mark in this regular expression denotes you are doing a lazy search.

## Author 

GitHub Username: Kriskris9
GitHub URL: https://github.com/Kriskris9

