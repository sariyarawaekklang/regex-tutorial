# Regex Tutorial - Matching an IP Address

Welcome to Regex Tutorial!

## Summary

Regular expressions, more commonly known as regex, are an pattern of characters that describe a certain amount of text. They can be used to obtain information from any text by searching for one or more matches of a specific search pattern. Fun fact: Regex can be used in almost all programming languages!
</br>
</br>
This Regex Tutorial will explain the component of regex in relation to matching an IP address, like shown in the following snippet:

```
^(([0-9]|[1-9][0-9]|1[0-9][0-9]|2[0-4][0-9]|25[0-5])(\.(?!$)|$)){4}$
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#author)

## Regex Components

### Anchors

Anchors are used to indicate the position of the numbers in the IP address. `^` is for the start of a string or line, as `$` is for the end of a string or line.

### Quantifiers

Quantifiers indicate how many times a character, group, or character class must be present in the input for a match to be found. The quantifier shown in this IP matching regex is `?`, which means that the preceding matches zero or one time.
<br/>
`123? matches a string that has 12 followed by zero or one 3.`

### OR Operator

OR operators are `|` and `[]`. `|` determines if a sequence matches a string and contains components of a previous string. `[]` deteremines that a sequence indeeds match a string, but does not contain components of a previous string.
</br>
`1(2|3) matches a string that has 1 followed by 2 or 3, and contains 2 or 3.`
</br>
`1[23] matches a string that has 1 followed by 2 or 3, but does not contain 2 or 3.`

### Character Classes

Character classes `.` are a special notation that matches any character from a certain sequence.

### Grouping and Capturing

Grouping and capturing `()` are a way to treat multipe characters as a single unit.
</br>
`(123) becomes 1 2 3.`

### Bracket Expressions

Bracket expressions, `[]` indicate a set of characters to match.
</br>
`[1-3] matches a string that has either 1 or 1 2 or 1 3. It is also the same as 1|2|3.`

### Greedy and Lazy Match

The greedy match used in the regex at the top is `{}`. Here, greedy match means matching the longest possible string.

## Author

Please feel free to reach out via [my GitHub](https://github.com/sariyarawaekklang) with any questions. Thank you for using my Regex Tutorial!
