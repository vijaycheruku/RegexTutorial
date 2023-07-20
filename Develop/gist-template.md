# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

### Anchors

- The characters ^ and $ are both considered to be anchors.
- The ^ anchor signifies a string that begins with the characters that follow it. An exact string match, such as ^Good, where the strings "Good" or "Good morning" match.
- The $ anchor is used to match an expression to its left at the end of a string. morning$ is an expression match to a string which ends with morining such as "good morning", " morning".

### Quantifiers

The quantifiers are used for specifying the number of occurrences of a character. Quantifiers set the limits of the string that your regex matches. They frequently include the minimum and maximum number of characters that your regex is looking for. 

Quantifiers include the following.

- ?— Matches the pattern zero or one time.
- +— Matches the pattern one or more times.
- *— Matches the pattern zero or more times.
- {x}- Specifies an expression to its left for only x times.
- {x, }- Specifies an expression to its left for x or more times.
- {x,y}- Specifies an expression to its left, at least x times but less than y times.


### Grouping Constructs

1. ( ) - It is used to match everything which is in the simple bracket.
2. The primary way you group a section of a regex is by using parentheses (()). Ex: (good):(morning) matches the string "good:morning"
3. Grouping constructs have two primary categories.
 - Capturing : capturing groups capture the matched character sequences for possible re-use.
 - Non-capturing : groups do not capture the matched character sequences for possible re-use. A grouping construct can be made non-capturing by adding the characters ?: at the beginning of an expression inside the parentheses.


### Bracket Expressions

- [ ] - It is used to match any character from a range of characters defined in the square bracket.
- Anything inside a set of square brackets ([]) represents a range of characters that we want to match.
- For example xz[atp]r is an expression which matches with the following strings: "xzar", "xztr", and "xzpr"


### Character Classes

1. A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match.

Character classes include the following.

- \s— match a one white space character.
- \S— match one non-white space character.
- \0— match a NULL character.
- \a- match a bell or alarm.
- \d- match one decimal digit, which means from 0 to 9.
- \D- match any non-decimal digit.
- \n- match a new line.
- \w- match the alphanumeric [0-9a-zA-Z] characters.
- \W- match a one non-word character
- \b- match a word boundary.


### The OR Operator
- (|) or [|] is the usage of or operator. | character indicates or operator.
- More precisely or operator can be explanied with the examples below.
  
  1. four|4: matches strings "four" or "4".
  2. a(b|c): matches a string that has a followed by b or c (and captures b or c).
  3. (a|b|c):(x|y|z) : both of the strings "abc:xyz" and "acb:xyz" would match, as well as "a:z", but "xyz:abc" would not match.

### Flags

Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex.

Most commonly used flags are:

 - g—Global search: the regex should be tested against all possible matches in a string.
 - i—Case-insensitive search: case should be ignored while attempting a match in a string.
 - m—Multi-line search: a multi-line input string should be treated as multiple lines

### Character Escapes

The backslash (\) in a regex escapes a character that otherwise would be interpreted literally. For example, the open curly brace ({) is used to begin a quantifier, but adding a backslash before the open curly brace (\{) means that the regex should look for the open curly brace character instead of beginning to define a quantifier. This is common when looking for strings with special characters that are the same as a particular component of a regex.

- It's important to note that all special characters, including the backslash (\), lose their special significance inside bracket expressions.



## Author

Vijay Cheruku

 Have Queries? Reach me at
 Email : vijay.cheruku@live.com
