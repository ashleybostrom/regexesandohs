# RegHexes && Ohs: Matching Hexadecimals in JavaScript

A tutorial on how the regular expression, or regex, works with descriptions of ALL components, each one in their respective section. This will be done in a GitHub gist rather than our traditional repository. A gist functions as a repository would and is created with Markdown similar to a README. This gist includes code examples, links, images, and everything else you would find in a README for a thorough and informative tutorial on how a regex is employed to match a hexadecimal (hex) value.

## Summary
A regular expression (regex) is a pattern that is used to match strings or their parts. For this instance of looking at how a regex works, we will go through how it is used in JavaScript to match a HEX value `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` in the outline below.

Before we get started, what is a hexidecimal? It is an alphanumeric code used to define sRGB ('s' signfies 'standard') colors that is implemented and read in computational and digital applications. Hex for short, the values represent our primary RGB (red, green, and blue) colors. As seen above the values have an optional `#` at the beginning of the string and contain a combination of either 6 or 3 characters, either capital or lowercase, of `a-f`, `A-F`, or `0-9`.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Conclusion](#conclusion)

## Regex Components

### Anchors
As the name implies, anchors signal to the beginning or the ending of the value string. In this example, we are using two anchors in our regex: `^` and `$`. The forward slash at the beginning of the string denotes a switch to the machine so it will know to read the value as is meant.

The `^` character signals the beginning of the string, while the `$` signals the end. To postulate, `^123` will match any string that begins with `123`, while `789$` will match any line ending in `789`.

A regex implements these characters to ensure a match of the full expresion between the anchors, from beginning to end.

### Quantifiers
A quantifier designates how many (quantity) characters are to be matched. Quantifiers follow the character(s) they designate. In this expression, our quantifiers are `?` and `{}`.  

The quantifier `?` means the character is optional, meaning it is to match 0 or 1 occurence(s). In this case, `#?` means the '#' symbol is optional, so a hexadecimal that doesn't have '#' in front is still a match.

The quantifier `{}` means we need to match the number of characters inside the curly brackets exactly. In this case, `{6}` means we need to match the 6 characters that came before, whereas it is the same with `{3}` only with the 3 preceding characters.

### The OR Operator

### Grouping Constructs


### Character Classes


## Conclusion 


## Author
