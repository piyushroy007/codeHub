## 58. Length of Last Word
https://leetcode.com/problems/length-of-last-word/description/?envType=problem-list-v2&envId=string

## Question 

    Given a string s consisting of words and spaces, return the length of the last word in the string.

    A word is a maximal 
    substring
    consisting of non-space characters only.

 

Example 1:

    Input: s = "Hello World"
    Output: 5
    Explanation: The last word is "World" with length 5.
    Example 2:

    Input: s = "   fly me   to   the moon  "
    Output: 4
    Explanation: The last word is "moon" with length 4.

## Solution : 

    int lengthOfLastWord(string s) {
        int count = 0 ;
        // start taking letters from the back of the string
        for(int i = s.size() - 1; i >= 0  ; i--){
            if(s[i] == ' ' && count != 0){
                    return count;
            } else if(s[i] != ' ' ){
                    count++ ;
            } else{
                continue ;
            }
        }
        return count ; 
    }