# sudoku
A widely known interesting game solved using backtracking!!
Problem: We have been given a sudoku as 2D array or matrix of dimension 9*9 with some intial values
and some empty values specified by 0. Now we have to fill all empty entries by some values such that
it maintains the property of sudoku. These Properties are:
1) All rows must have unique entries
2) All columns must have unique entries
3) Withing An Square of size 3*3 all entries must be unique(see below  example for more clearity).

Initial State of Sudoku:

| 7 8 0 | 4 0 0 | 1 2 0 |
| 6 0 0 | 0 7 5 | 0 0 9 | 
| 0 0 0 | 6 0 1 | 0 7 8 | 
-------------------------
| 0 0 7 | 0 4 0 | 2 6 0 | 
| 0 0 1 | 0 5 0 | 9 3 0 | 
| 9 0 4 | 0 6 0 | 0 0 5 | 
-------------------------
| 0 7 0 | 3 0 0 | 0 1 2 | 
| 1 2 0 | 0 0 7 | 4 0 0 | 
| 0 4 9 | 2 0 6 | 0 0 7 |

A Sovled State for above example will look like:

| 7 8 5 | 4 3 9 | 1 2 6 | 
| 6 1 2 | 8 7 5 | 3 4 9 | 
| 4 9 3 | 6 2 1 | 5 7 8 | 
-------------------------
| 8 5 7 | 9 4 3 | 2 6 1 | 
| 2 6 1 | 7 5 8 | 9 3 4 | 
| 9 3 4 | 1 6 2 | 7 8 5 | 
-------------------------
| 5 7 8 | 3 9 4 | 6 1 2 | 
| 1 2 6 | 5 8 7 | 4 9 3 | 
| 3 4 9 | 2 1 6 | 8 5 7 | 

Approach: We can solve this problem by trying each and every number for every empty position but time complexity for this method is O(9^N^2) where N is dimension of 

