Question: https://www.geeksforgeeks.org/count-ways-reach-nth-stair/

Count ways to reach the n’th stair

There are n stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs at a time. Count the number of ways, the person can reach the top.

Input: n = 1
Output: 1
There is only one way to climb 1 stair

Input: n = 2
Output: 2
There are two ways: (1, 1) and (2)

Input: n = 4
Output: 5
(1, 1, 1, 1), (1, 1, 2), (2, 1, 1), (1, 2, 1), (2, 2)


This is my reasoning and attempt at solving the problem:

1. define my base cases
  if N < 1 return 0
  if N === 1 return 1
  if N === 2 return 2

2. define the simplest combos:
 if all 1 step
 if all 2 steps

3. think of a way to force swaps between the two simplest combos
 3 a. keep track of all these swaps
 3 b. think of a way to know how many time to swap

4. convert all combos to a set and count set length
 - reasoning: assuming we cannot solve for how to keep track of swaps we can eliminate duplicate combos by converting the storage of combos into a set
