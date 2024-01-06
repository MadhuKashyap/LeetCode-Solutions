### Search a 2D Matrix
You are given an m x n integer matrix matrix with the following two properties:

Each row is sorted in non-decreasing order.
The first integer of each row is greater than the last integer of the previous row.
Given an integer target, return true if target is in matrix or false otherwise.

You must write a solution in O(log(m * n)) time complexity.

Example 1:


![image](https://github.com/MadhuKashyap/LeetCode-Solutions/assets/40714383/c588c84b-fce6-4bc9-856a-b450ab14a085)

```
Input: matrix = [[1,3,5,7],[10,11,16,20],[23,30,34,60]], target = 3
Output: true
```
Example 2:


![image](https://github.com/MadhuKashyap/LeetCode-Solutions/assets/40714383/e9dc3c70-bcf4-428c-b9f0-f05e893a9540)

```
Input: matrix = [[1,3,5,7],[10,11,16,20],[23,30,34,60]], target = 13
Output: false
``` 

Constraints:

* m == matrix.length
* n == matrix[i].length
* 1 <= m, n <= 100
* -104 <= matrix[i][j], target <= 104
