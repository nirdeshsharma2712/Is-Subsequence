# 📊 LeetCode Problem: Is Subsequence

## 🧩 Problem Statement

Given two strings `s` and `t`, return `true` if `s` is a **subsequence** of `t`, or `false` otherwise.


> **Note :**
> - A subsequence of a string is a **new string** that is formed from the **original string** by deleting some (can be none) of the **characters** without disturbing the **relative positions** of the remaining characters. (i.e., "ace" is a subsequence of "abcde" while "aec" is not).


## 🧠 Approach: Two-Pointer Logic

- Use two pointers i (for s) and j (for t).

- Traverse t:

> - If s[i] == t[j], move both.
> - Else, move j only.

- At the end, if i == s.length() → ✅ it's a subsequence.





## ✅ Example Walkthrough

### Example 1

##### Input: s = "abc", t = "ahbgdc"
##### Output: true


### Example 2

##### Input: s = "axc", t = "ahbgdc"
##### Output: false



## 🛠️ Constraints

- `0 <= s.length <= 100`
- `0 <= t.length <= 10^4`
- `s` and `t` consist only of lowercase English letters.
