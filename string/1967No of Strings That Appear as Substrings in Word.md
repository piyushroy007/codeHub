https://leetcode.com/problems/number-of-strings-that-appear-as-substrings-in-word/description/

## 1967. Number of Strings That Appear as Substrings in Word

Given an array of strings patterns and a string word, return the number of strings in patterns that exist as a substring in word.
A substring is a contiguous sequence of characters within a string.

## Example 1:

Input: patterns = ["a","abc","bc","d"], word = "abc"
Output: 3
Explanation:

-   "a" appears as a substring in "abc".
-   "abc" appears as a substring in "abc".
-   "bc" appears as a substring in "abc".
-   "d" does not appear as a substring in "abc".
    3 of the strings in patterns appear as a substring in word.

## Example 2:

Input: patterns = ["a","b","c"], word = "aaaaabbbbb"
Output: 2
Explanation:

-   "a" appears as a substring in "aaaaabbbbb".
-   "b" appears as a substring in "aaaaabbbbb".
-   "c" does not appear as a substring in "aaaaabbbbb".
    2 of the strings in patterns appear as a substring in word.

## Solution in C++ :

    int numOfStrings(vector<string>& patterns, string word) {
        int count = 0;
        for(int i=0; i<patterns.size(); i++){
            if(word.find(patterns[i]) <= word.size() ){
                count++;
            }
        }
        return count;
    }
