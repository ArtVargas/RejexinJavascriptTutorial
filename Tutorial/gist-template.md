# Chapter 1 By Art Vargas: Matching A Hex Value Regex

Thank you and welcome to this comprehensive tutorial in regards to understanding and following the concept of Regex which is also known as regular expressions that are used to search through various data which will then find strings that fit within a certain given parameter. Upon learning and completing this tutorial you will have an absolute clear understanding of r components which will be demonstrated with proper comprehension and vocabulary in order to give detailed explanations which can later be used to break apart components which will solely be focused on the topic of Regex being able to be assisted with hex values.



## Summary

Throughout the tutorial being demonstrated that will feature regular expressions also known as regex there will be various references and examples that will further demonstrate an analysis in regards to each regex component that will be able to provide new time coders or students with the basic understanding of all various components. The information of Hex Values will be the primary topic of discussion and study for further analysis. The knowledge stated before will showcase the use of regex being able to further assist in hexadecimal data. The standard Regex would demonstrate: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/. The necessary Regex components such as anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and character escapes will be discussed and explained for further analysis.





## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)


## Regex Components

### Anchors

A Regex anchor is the start and end of the string which makes it so the Regex matches the string we are looking for.

The anchors for our Regex are the ^ and $ characters. This will indicate that the #?([a-f0-9]{6}|[a-f0-9]{3}) between the ^ and $ is what we will be looking for in this case.

 Anchors can provide a way to limit how a regex matches a particular string by telling the regex engine where matches can begin and when they can end. With the use of anchors you will be provided with more flexibility with simple constructs that will provide a degree of control which you weren’t provided with before 


### Quantifiers

In regular expressions, quantifiers are metacharacters that specify how many times the previous character or group should be matched. Quantifiers will allow you to specify the number of occurrences of a character or group which will make the process of matching patterns with varying lengths much more simpler. For our Regex, ? is the preceding quantifier which in terms states that the preceding character is options. This will indicate that the  # in the Regex is optional, and in 6 character hex codes. 
Example: #FF0000 OR FF0000.
The ? means that there can be a 0 or 1 occurrence which will either show up all at once or not at all and if the string starts with  # it will be matched but, even without including the  #, it will still match if it follows the other quantifiers. Other 2 quantifiers are {6} and {3}. These set character amounts that the Regex looks to match with since in this case hex values can come in 6 characters (#FF0000) or 3 characters (#F00).

### OR Operator

The OR Operator allows you to search for 2 different matches which will essentially match 1 or match 2.
In our Regex: [a-f0-9]{6}|[a-f0-9]{3}, the OR operator is in the middle. It is looking to match 6 characters with a character class of a-f0-9, or in this case 3 characters with a character class of a-f0-9.

### Character Classes

Character classes are very much intertwined with bracket expressions. Inside the bracket expression is the Character Class which determines the characters and numbers that will be used for matching. The most basic form of a character class is to simply just place a set of characters side-by-side within square brackets. For our Regex `[a-f0-9]``, a-f because hex values use a-f and don’t go to z. 0-9 are the numbers that will be primarily used in hex codes so that the given numbers will match.


### Flags

Flags in Regex are used to add extra parameters needed such as case-sensitive matching (i), which will search for all matches instead of just one. In the Regex being demonstrated there is no flag being shown by having no letters at the end of /^#?([a-f0-9]{6}|[a-f0-9]{3})$/.
By having no flags that means our Regex is case sensitive and since its a-f is lowercase in the regex that means it will be then looking for lowercase letters to match.
If we wanted enable the inclusion of making it not case sensitive as a further example  we would add  i to the end of the Regex,  /^#?([a-f0-9]{6}|[a-f0-9]{3})$/i

### Grouping and Capturing

Grouping constructs are what sets the sub expression which is always known as the matched string. They are usually shown with parentheses. In the code that we will use, [a-f0-9]{6}|[a-f0-9]{3}The subexpression is what is resting inside of the given parenthesis. 
[a-f0-9]This sets the character set which will then be used for matching. A-F are being used by the hex values and will not go to Z. 0-9 are the numbers indicated which will be used in hex codes that our numbers will be looking to match with.

### Bracket Expressions

Bracket expressions are an expression that are set within brackets. It’s self explanatory in the name but they add great value due to setting the character and number set that the Regex will then match with.
Example: [a-f0-9]{6} This will set the character and will be then used for matching the hex values that are essentially 6 characters long. [a-f0-9]{3}This will set the character that will be used for matching containing hex values that are only 3 characters long in this example.

### Greedy and Lazy Match

As to be expected the definition of a greedy match indicates that a search will try to find the longest and possible string whereas a lazy match will do the complete opposite and find the smallest possible given string.
Greedy Quantifiers Examples:
One or more revised gist
Zero or More
{2,4} = Two to four times as a greedy lazy quantifier
The expression: https?:\/\/)? Uses the lazy match of? Which is looking for http or https [Example:] [a-zA-Z0-9()]{1,6}is looking for a-z and is also looking for 0-9; which will be one to six times as greedy. You take the basic information given and acknowledge the greedy match/ lazy match that is directly provided with the given possible string that is showcased.

### Boundaries

Boundaries are similar to an anchor such as in the way they used the expression /b for word boundaries and /B for non-word boundaries. They are a zero-length match that marks the beginning and end of a numerical sequence that makes it much easier to find the whole words needed for expression values. 
Example:  \b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)is searching for a whole word or digit in the expression provided as an example of analysis and discussion.

### Back-references

Back references are filters used to match the same text which is previously matched by a capturing group. A notable example would be when you need to search for a repeated word, the first match given could possibly use a pattern that extracts a single word. The second would back reference that refers to the captured group that was given to the word extraction.


## Author

Hello! I am Art Vargas. I am currently studying Full Stack Web Development in the UTSA Bootcamp here in San Antonio, TX. Any additional questions or concerns please feel free to contact me!

Follow me on GitHub: 

Deployed GitHub-Gist Link:

GitHub Repository Link: 

