# software-quality-handbook
# Coding Standards

Coding standards are collections of rules and guidelines that determine the programming style, procedures, and methods for a programming language.

### Importance of Coding Standards

Without coding standards, every individual in a team will use their own coding styles. 
It will not be easy to maintain and will be difficult to debug the code.

## Formatting

Code formatting allows programmers to vaguely convey what their code intends to do. 
Code formatting is often a programmer's reader's first encounter with their system. 
It deserves attention and care.

### Components That Affect Code Formatting:

* Quick Readability: The reader should be able to understand the gross structure of the code in a glimpse. 
  The shapes made by blocks of text help you communicate the overall structure.

* Detailed Readability: The reader must be able to read lots of code in depth.

* Length: The number of lines must be minimized so that browsers can be as small as possible.

* Width: The width of code must be minimized. Code must not ordinarily spill across the right margin, 
  requiring horizontal scrolling or destroying the shape of the text with line wrapping.

### Essential Parts of Code Formatting

Conventions have been made to make sure code is as understandable as possible. 
This helps avoid errors, troubleshoot problems and makes maintaining someone else’s (or even your own) work much easier.

There are differing conventions depending on the language that you are using. 
Yet, all of them basically revolve around the following:

1. Indentation 
2. White space
3. Capitalization and naming conventions
4. Style and spelling of functions, variables and more
5. Use and style of comments

## Naming Conventions

 A naming convention is a set of rules for choosing the character sequence to be used for identifiers 
 which represent variables, types, functions, and other entities in source code and documentation.

### Significance of Naming Conventions

It is important for programmers to utilise and agree on naming conventions instead of allowing everyone
to choose any character sequence.

The following are reasons why: 

* To reduce the effort needed to read and understand source code
* To enable code reviews to focus on more important issues than arguing over syntax and naming standards.
* To enable code quality review tools to focus their reporting mainly on significant issues other than syntax and style preferences.

### Potential Benefits 

Some of the potential benefits that can be obtained include the following:

* to help formalise expectations and encourage consistency within a development team;
* to enable the use of automated refactoring or search and replace tools with minimal potential for error;
* to enhance clarity in cases of potential ambiguity;
* to help avoid "naming collisions" that might occur when the work product of different organisations is combined.
* to provide meaningful data to be used in project handovers which require submission of program source code and all relevant documentation;
* to provide better understanding in case of code reuse after a long interval of time.

## References

* [Code Formatting Guide](https://torquemag.io/2019/07/code-formatting-guide/)
* [Java Style Guide](https://google.github.io/styleguide/javaguide.html#s4-formatting)
* [Code Formatting Patterns](http://c2.com/ppr/formatting.html#6)
* [Naming Conventions](https://en.wikipedia.org/wiki/Naming_convention_(programming)#:~:text=In%20computer%20programming%2C%20a%20naming,in%20source%20code%20and%20documentation)
