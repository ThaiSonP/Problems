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
