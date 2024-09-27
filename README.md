# String Calculator

## Description:

Create a C# function called Add that takes a string of numbers as input and returns their sum as an integer.

## Requirements

- The input string can contain zero, one, or multiple numbers separated by commas (,).
- Allow the Add function to handle new lines between numbers (i.e., \n).
- Numbers greater than 1000 should be ignored.
- Negative numbers will throw an exception with the message "Negatives not allowed" followed by a list of the negative numbers that were found.
- Support different delimiters. To change a delimiter, the beginning of the string will contain a separate line that looks like this: //[delimiter]\n[numbers…]. For example, //;\n1;2 should return 3 where the delimiter is ;.   
- Delimiters can be of any length with the following format: //[delimiter]\n. For example: //***\n1***2***3 should return 6.

## Example Test Cases:

- Add("") should return 0
- Add("1") should return 1
- Add("1,2") should return 3
- Add("1\n2,3") should return 6
- Add("1001,2") should return 2
- Add("-1,2") should throw an exception "Negatives not allowed: -1"
- Add("2,-4,3,-5") should throw an exception "Negatives not allowed: -4,-5"
- Add("//;\n1;2") should return 3
- Add("//***\n1***2***3") should return 6
