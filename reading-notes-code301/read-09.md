# Read-08, 23 Feb 2021, Code 301

## Functional Programming 

![functional programming](https://www.leadingagile.com/wp-content/uploads/2018/02/When-functional-programming-isnt.jpg)

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

**pure functions**
- Not causing any side effects 
- It returns the same result if given the same arguments (cannot use global objects they all must be arguments)

**Restriction**

- If our function reads external files, it’s not a pure function — the file’s contents can change.
- Any function that relies on a random number generator cannot be pure.
- It does not cause any observable side effects (like modifying global array 

[GitHublink](https://omar-tarawneh.github.io/reading-notes/reading-notes-code301/read-09)