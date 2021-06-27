# Regex_with_Python
Pythonic approach to very basic regular expressions. 
This code was written as an assignment to wirte a programatic approach to accomodate for regular expressions. 

The task(s) that this jupyter notebook accomplishes are as follows:
 
 1. Take a 'search' input formatted with regex functionalities 
 using the following boolean operators:
     a. AND
     b. OR
     c. NOT
     d. /n (proximity operator)
     
 eg.  ((confidential OR proprietary) /3 information) AND NOT (required disclosure)
 
 2. Take a 'text' input containing the text
 to search.
 
 3. Output a boolean (in this case True or False) if the search criteria is satisfied by the text. 

 Assumptions made: The assumptions made based on the wording of the assignment
 are the following:
     
     a. Only the following boolean operators can be used:
         - AND
         - OR
         - NOT
         - /n (proximity)
     b. The user will be entering the text manually. It will not be read from a 
     file from the system or other repository
     c. True and False are the only desired outputs for this function with 
     a True value indicating the regex search term was found in the entered text 
     and a False value indicating otherwise.

Known Issues with the code as written: 

There are known issues with the code as it is currently written: 
    
    1. Unfortunately, I was unable to figure out how to make the search work
    on a standalone parentheses basis. For example, if one were to enter 
    (apple OR pie) as a search term, the first parentheses will cause an 
    error because of lines 21 to 27 programatically resulting in a list rather than a string. 
    
    2. The operators (AND, OR, NOT) ARE NOT case agnostic. They MUST be in all
    caps in the search entered. 
