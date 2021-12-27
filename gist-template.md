# The World of Regex

Regular expression, also known as "Regex" for short, is a sequence of characters that one can utilize to specify search patterns for any string of characters or text. 

Regex is a useful tool in cases of searching through the text to change something or for user validation. For instance if a username needs a certain amount of letters or an @ symbol, we can validate it with some Regex code. Regex is used like a booleon and it is used to keep our data clean.


## Summary
In this tutorial we will be examining the following Regex:
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

The regex above is used to search for and match a url. In the following sections, we will examine each piece of this regex to understand how the individual pieces come together to enter in a valid url. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Boundaries](#boundaries) 


### Anchors
Anchors are elements of regex expressions that indicate position. In the code above there are two anchors. 
So in the URL matching example the ^ is the anchor for the expression.
'^' is a string anchor and signifies the start of the regex expression. 

 `$` - the dollar-sign symbol indicates to the engine to match any string that ends with the preceding characters.

### Quantifiers
Quantifiers are elements of regex that indicate how many times a character, character class, or group should be present. 
Some quantifiers used in the code are as follows:

*: Repeats the previous item 0 or more times

?: it makes the preceding code optional, also known as a greedy quantifier so if it does show up there is no issue
ex: (https?:\/\/)?

+: it will repeat the previous item once or more 

{}: {num} or {min, max} --will take in an amount or certain amount you want to put 
ex: in the regex above it is {2,6}
So we are only accepting input from 2-6 characters. 

### Character Classes
Character Classes are elements of regex that appear between square brackets, `[]`. By using the square brackets, `[]`, we are telling the engine to match any of the characters within the brackets.
ex: [a-z\.] 
This matches a character in the range of 'a' to 'z', a '/' and a period.  

### Grouping and Capturing
Regex can also include groupings, as indicated by the `()`.
 Whatever characters are placed within round parentheses `()` will be part of a group. 
Quantifiers can be applied to groupings, or groupings can also be used to create numbered capture groups. 

### Boundaries
Every regex expression will have boundaries, as indicated by a forward-slash `/` and will end with a `/`. 

Regex expressions are stored in forward slashes /(inside of the slash will be regex code /. 
We can also use flags which can help us search for specific things while working on our regex.  

### Author
Mohammad Ibrahim is a student at Colombia University coding bootcamp and enjoys to code. He plays sports on his free time and loves coffee. 
- https://github.com/mibrahim234