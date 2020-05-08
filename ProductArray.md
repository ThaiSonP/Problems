This problem was asked by Uber.

Given an array of integers, return a new array such that each element at index i of the new array is the product of all the numbers in the original array except the one at i.

For example, if our input was [1, 2, 3, 4, 5], the expected output would be [120, 60, 40, 30, 24]. If our input was [3, 2, 1], the expected output would be [2, 3, 6].

Follow-up: what if you can't use division?


// thought process in solution
repl link: https://repl.it/repls/RubberyNiftyObservation

time complexity 2N = > N 
 i am using two for loops to iterate through the array 
    first for loop is to find the product of all the integers
    second for loop is is dividing the product by the index then pushing it to the solution array
    
-attempted to use a nested for loop and found out the time complexity was longer than two seperate for loops

//attempt #2

  for (let i = 0; i <ary.length;i++){
    let product = 1
    
    for (let j = 0; j <ary.length;j++){
      if(ary[i] === ary[j]){ continue }
       n+=.001
      product = product * ary[j]
    }      
   solution.push(product)
  } 
  
  using a nested for loop to skip product rather than using division - time complexity is N^2 
