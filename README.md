```
DAA-IT-2223P
Design and Analysis of Algorithms Practical
Day 02

1. String Concatenation
------------------------

str1 = 'apple';
str2 = 'banana';
result = strcat(str1, str2);
strcat() combines multiple strings end to end.

This will give: 'applebanana'.

marks = {'hello', 'world', 'sri'};
result2 = strcat(marks{:});
Concatenates all elements in a cell array into one string.

Output: 'helloworldsri'.  
 
result3 = strjoin(marks, ':');
Joins the array with a colon : separator.

Output: 'hello:world:sri'.

2. String Comparison
--------------------
 
wstr1 = 'age';
wstr2 = 'age';
result4 = strcmp(wstr1, wstr2);
strcmp() checks if the strings are exactly equal.

Output: 1 (true) if they are the same, otherwise 0.

3. Finding and Replacing Substrings
-----------------------------------
 
stril = 'the cat sat on the mat';
indic = strfind(stril, 'cat');
strfind() returns the starting index of the substring 'cat'.

Here, it will return 5.

old = 'cat';
new = 'dog';
replace = strrep(stril, old, new);
strrep() replaces 'cat' with 'dog'.

Output: 'the dog sat on the mat'.

4. Splitting Strings
--------------------
 
inputstring = 'apple,banana,orange,grapes';
substring = strsplit(inputstring, ',');
strsplit() breaks a string into parts using a delimiter (here, a comma).

Output: {'apple', 'banana', 'orange', 'grapes'}.

5. Case Conversion and Trimming
-------------------------------- 

st1 = 'appLE';
lowercase = lower(st1);    % Converts to lowercase: 'apple'
uppercase = upper(st1);    % Converts to uppercase: 'APPLE'
  
 
trim = strtrim(' hello world ');
strtrim() removes leading and trailing spaces.

6. Grading System Based on Marks
--------------------------------

marks = input('Enter the marks : ');
Takes marks as input.

Checks the range and displays the corresponding grade (A+, A, B, C, D, F).

Also checks if the input is invalid (>100).

7. Largest of Three Numbers
----------------------------

num1 = input('Enter the number 1: ');
num2 = input('Enter the number 2: ');
num3 = input('Enter the number 3: ');
Uses if-elseif to compare and print the largest number among three.

8. Vowel or Consonant Check
---------------------------- 
  
letter = input('Input the letter : ','s');
Accepts a single character.

switch-case checks if it is a vowel (a, e, i, o, u).

Otherwise, prints 'Consonant'.





