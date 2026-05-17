# Reverse String - LeetCode Solution

This repository contains my Java solution for the **Reverse String** problem from LeetCode.

## Problem Link
https://leetcode.com/problems/reverse-string/

## Problem Statement
Write a function that reverses a string represented as a character array `char[]`.

The solution should modify the input array directly.

---

## My Approach

In this solution:

- I created a clone of the original character array
- Traversed the cloned array from the end
- Stored characters back into the original array in reverse order

---

## Java Solution

```java
class Solution {
    public void reverseString(char[] s) {

        char arr[] = s.clone();

        int count = 0;

        for(int i = s.length - 1; i >= 0; i--) {

            s[count] = arr[i];
            count++;
        }
    }
}
Example

Input:

['h','e','l','l','o']

Output:

['o','l','l','e','h']
Concepts Used
Arrays
Strings
Traversing Arrays
Cloning Arrays
Time Complexity
O(n)
Space Complexity
O(n)

Extra space is used because of the cloned array.

Learning Outcome

Through this problem, I practiced:

Array cloning in Java
Reverse traversal
In-place modification of arrays
String manipulation concepts

⭐ Consistently practicing DSA and uploading solutions to GitHub.
