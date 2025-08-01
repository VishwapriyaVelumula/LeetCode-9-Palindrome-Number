# LeetCode-9-Palindrome-Number
Given a signed integer x, return true if it reads the same forward and backward (a palindrome), otherwise return false. Do this without converting the number to a string and in O(log x) time and O(1) space.


# LeetCode9 – Palindrome Number

## Problem Statement
Determine whether a given 32-bit signed integer is a palindrome. Negative numbers and numbers ending in zero (except 0 itself) are not palindromes.

## Approach
- Reject negative inputs immediately.
- Reverse the digits of the number using modulus (`% 10`) and division (`/ 10`) into a temporary variable.
- Compare the reversed value to the original.
- Return `true` if they match, else `false`.

## Time Complexity
O(log x) — each iteration removes one digit.

## Space Complexity
O(1) — only constant extra variables used.

## Examples
- Input: `121` → Output: `true`  
- Input: `-121` → Output: `false`  
- Input: `10` → Output: `false`
