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
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

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

### Grouping and Capturing

### Bracket Expressions

Bracket expressions are an expression that are set within brackets. It’s self explanatory in the name but they add great value due to setting the character and number set that the Regex will then match with.
Example: [a-f0-9]{6} This will set the character and will be then used for matching the hex values that are essentially 6 characters long. [a-f0-9]{3}This will set the character that will be used for matching containing hex values that are only 3 characters long in this example.

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
