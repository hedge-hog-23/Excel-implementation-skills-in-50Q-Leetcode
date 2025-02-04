# Intuition
<!-- Describe your first thoughts on how to solve this problem. -->
Just traverse from reverse of the string and find the length of last word.

# Complexity
- Time complexity:
$$O(n)$$

- Space complexity:
$$O(1)$$

# Code
```python3 []
class Solution:
    def lengthOfLastWord(self, s: str) -> int:
        res = 0
        for i in range(len(s)-1,-1,-1):
            if(s[i] != ' '):
                res+=1
            elif(res > 0):
                break
        return res
        
```
