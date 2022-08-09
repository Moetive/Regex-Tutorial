# Regular Expressions Tutorial



## Summary

The purpose of this tutorial is to understand the concept of regular expressions (Regex)
For example, the following regular expression can be used to verify that user input is a valid email address:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

    Anchors decide what position the characters are in
    ^ – The caret anchor matches the beginning of the text.
    $ – The dollar anchor matches the end of the text.

### Quantifiers
Quantifiers tell ou how many characters, classes, groups there needs to be for to find a match
They can be catergorized as "greedy" and "lazy" 
`x*`
`x+`
`x?`
`x{n}`
`x{n,}`
`x{n,m}`
`x*?`
`x+?`
`x??`
`x{n}?`
`x{n,}?`
`x{n,m}?`
### Grouping Constructs
`(x)` The "()" matches the x and captures it.
`(?<Name>x)` The "<>"  matches x and stores it under the name of <name>.
`(?:x)` This matches the x but does not remember that it was matched.
`\n` This uses the last substring matching the "n" to match
`k<Name>` this uses the capture group specified by <Name> to match
### Bracket Expressions

`[ ]` Brackets determine how many characters to match. If an individual character is within the brackets it will match.
`{ }` Characters in the Curly brackets determine an exact amount of characters to match
`( )` Parentheses are used to remember matches as explained above in grouping constructs
### Character Classes
Character classes match characters from particular set.
Types: 
`[xyz] [a-c]` 
`[^xyz] [^a-c]`
`.`
`\d`
`\D`
`\w`
`\W`
`\s`
`\S`
`\t`
`\r`
`\n`	
`\v`
`\f`	
`[\b]`	
`\0`	
`\cX`	
`\xhh`	
`\uhhhh`	
`\u{hhhh} or \u{hhhhh}`	
`\p{UnicodeProperty}, \P{UnicodeProperty}`
`\`
`x|y`	

### The OR Operator
` | ` Use the | operator to match characters and expressions from either side of the | operator
### Flags
The use of flags are option but we can use flags for the following:
`g` match a pattern 
`i` makes a regular expression case insensitive
`m` Multi-line mode to utilize and match with ` ^ $ ` anchors 
`u` enables unicode
`s` disables multi-line mode by matching by new lines of characters
### Character Escapes
Backslash in regex are used to escape for example `/x\*c/` — the backslash "escapes" the `*`
`\s` Are used for spaces
`\w` Are used for word characters

## Author
#Mohamed Omar
[GitHub](https://github.com/Moetive)
[LinkedIn](https://www.linkedin.com/in/moetive/)
