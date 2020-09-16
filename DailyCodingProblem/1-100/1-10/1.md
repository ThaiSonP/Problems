This problem was recently asked by Google.

Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

For example, given [10, 15, 3, 7] and k of 17, return true since 10 + 7 is 17.

Bonus: Can you do this in one pass?

*attempt at solving problem
https://repl.it/repls/ReadyAdequateLists

thought process:
1  - edgecases - the function NEEDS to add two items together.
2  - I am using a for loop to iterate through each index. 
2b - Subtracting the element from k (the sum) THEN  check if that difference is included in the array.
2c - There might be an easier way by splitting the array in a sorted order because there wouldn't be a need to go through ALL the indexes if most of the items have been discluded in the find
