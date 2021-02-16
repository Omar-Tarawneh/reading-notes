# Read-04, 17 Feb 2021, Code 301

# Responsive Web Design and Regular Expressions

## Responsive Web Design

_The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning._

![grid](https://devopedia.org/images/article/179/2142.1559055827.jpg)

code for Container:
```css
.container  {  display: grid | inline-grid;  }
.container  {  grid-template-columns:  ... | ...;  grid-template-rows:  ... | ...;  }
.container  {  grid-template-columns:  40px  50px auto 50px  40px;  grid-template-rows:  25%  100px auto;  }
```

code for Children:
```css
.item  {  grid-column-start: <number> | <name> | span <number> | span <name> | auto;  grid-column-end: <number> | <name> | span <number> | span <name> | auto;  grid-row-start: <number> | <name> | span <number> | span <name> | auto;  grid-row-end: <number> | <name> | span <number> | span <name> | auto;  
grid-column: <start-line> / <end-line> | <start-line> / span <value>;  grid-row: <start-line> / <end-line> | <start-line> / span <value>;
}
```

# Regular Expressions

**RegExp Object**

_A regular expression is an object that describes a pattern of characters._

_Regular expressions are used to perform pattern-matching and “search-and-replace” functions on text._

**Special characters in regular expressions.**

Characters / constructs

Corresponding article

`\`,  `.`,  `\cX`,  `\d`,  `\D`,  `\f`,  `\n`,  `\r`,  `\s`,  `\S`,  `\t`,  `\v`,  `\w`,  `\W`,  `\0`,  `\xhh`,  `\uhhhh`,  `\uhhhhh`,  `[\b]`

Character classes

`^`,  `$`,  `x(?=y)`,  `x(?!y)`,  `(?<=y)x`,  `(?<!y)x`,  `\b`,  `\B`

Assertions
`(x)`,  `(?:x)`,  `(?<Name>x)`, `x|y`,  `[xyz]`,  `[^xyz]`,  `\_Number_`

Groups and ranges
`*`,  `+`,  `?`,  `x{_n_}`,  `x{_n_,}`,  `x{_n_,_m_}`

Quantifiers
`\p{_UnicodeProperty_}`,  `\P{_UnicodeProperty_}`

[github page Link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code301/read-04)
