---
name: Bug report (English)
about: Create a bug report to help us improve our content.
title: 'test case missing for 1166'
labels: 'missing test case / wrong test case'
assignees: ''

---

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->

#### Your LeetCode username
<!-- Your LeetCode username -->
xwshiba


#### Category of the bug
- [ ] Question
- [ ] Solution
- [ ] Language
- [x] Missing Test Cases 


#### Description of the bug
<!-- A clear and concise description of what the bug is. -->
Question [1166. Design File System](https://leetcode.com/problems/design-file-system/)
The description suggests that "For example, "/leetcode" and "/leetcode/problems" are valid paths while an empty string "" and "/" are not."
This means when we input "/" the result should return false instead of true. Currently it's returning true.
Case 1:
```
["FileSystem","createPath"]

[[],["/",1]]
```

Case 2:
```
["FileSystem","createPath","createPath","createPath","get","createPath","get"]
[[],["/leet",1],["/leet/code",2],["/leet/code",2],["/leet/code"],["/c/d",1],["/c"]]
```


#### Code you used for Submit/Run operation
<!-- 
Please make sure you wrap your code with ``` tags. 
Otherwise we may reject your request. 
-->


```
["FileSystem","createPath"]
[[],["/",1]]
```
This below should be included.
```
["FileSystem","createPath","createPath","createPath","get","createPath","get"]
[[],["/leet",1],["/leet/code",2],["/leet/code",2],["/leet/code"],["/c/d",1],["/c"]]
```

#### Language used for code
<!-- C++ -->
Python


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
Case 1: I think the test case should return `[null, false]` instead of `[null, true]`.
Case 2: This one should be included.



#### Screenshots
<!-- If applicable, add screenshots to explain your issue. -->

![image](https://user-images.githubusercontent.com/64823359/165887852-6f153c68-d796-46f2-bfd8-8bde988c6551.png)


#### Additional context
<!-- Add any other additional context about the bug. -->
