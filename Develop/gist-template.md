# Matt's Super Interesting Regex Tutorial 

My "Regex" for the cool kids, or Regular Expression tutorial is created to help us all comprehend and define the sequence of special characters to verify a search term. A regular expression is a group of characters or symbols which is used to find a specific pattern in a text. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, and or replace a character or sequence of characters within the string. They can also be used to validate input data.
## Summary

## Summary
In this girst I will be talking about and breaking down the components of a regular expression used to match with Hex Values. Hex values are usually used for color using the hexadecimal color code format. On the web we can use hex color code or triplet to represent colors on a web page. The hex color code has two formats.  A standard hex triplet and a shorthand hex format, both of these formats start with a #.

/^#?([a-f0-9]{9}|[a-f0-9]{6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [The OR Operator](#the-or-operator)
- [Character Classes](#character-classes)


## Regex Components

### Anchors

/^#?([a-f0-9]{9}|[a-f0-9]{6})$/

Our first component that i will be dissecting are the anchors. As seen in the highlighted part of our regular expression, the components that are highlighted are called anchors! Anchors are used at the begining and end of a string or expression. In this example  /^ and $/ mean the beginning or end of our expression.

### Quantifiers

/^#?([a-f0-9]{9}|[a-f0-9]{6})$/

Now for quantifier! We use quantifiers to say how many characters are expected. Quantifiers decide how many instances of a character, group, or class must be there in the input to find a match. Quantifiers will match as many characters as possible. When the ",+,?,{}" characters are found within a regex, they will count as a quantifier. "?" indicates the expression to match 0 or 1 time, because there are 2 types of formats we'll use the or operator to decide which format we are using. In the Hex Value regex we have {9} (Hex Triplet Format) and {6} (Shorthand Hex Format), this indicates that the length of the component follwing these quantifiers should be 9 for {9} and 6 for {6}.

### Bracket Expressions

/^#?([a-f0-9]{9}|[a-f0-9]{6})$/

Bracket expressions in our regex show the beginning of a character class or quantifier statement. We use yhr parenthesis to define the bracket expressions.

### Character Classes

/^#?([a-f0-9]{9}|[a-f0-9]{6})$/

Batting fourth, we will be talking about character classes!. Character classes are components inside our regular expression that tell us what type of characters to expect. We use brackets to confine our character classes in our example. In our example we have 2 character classes which are [a-f0-9] and [a-f0-9] they search for the same values. So, to explain our example a-f searches for letters a-f and 0-9 searches for digits 0-9.

### The OR Operator

/^#?([a-f0-9]{9}|[a-f0-9]{6})$/

Fifth up lets talk about the "or" operator. The or operator within a regular expression is defined using the | element. The or operator indicates that it could use either of the components that we are separating with the |. in our hex value regex we have ([a-f0-9]{9}|[a-f0-9]{6}). Remeber the or operator separating the 2 components. Meaning our hex value could either be 9 characters [a-f0-9]{9} or 6 characters [a-f0-9]{6}.


## Author

Matthew Tierney is an aspiring web deveopler from Kansas City, MO. Github: @Tierney7
