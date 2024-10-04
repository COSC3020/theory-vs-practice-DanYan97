# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asympotic analysis ignored the constant factor and lower-order terms, in the
  real world practical scenarios with finite input, these factos can impact the
  performance significantly.
  2. Asympotic analysis is a theoretical model, it does not account for the real-world
  hardware, such as CP cache size, memory bandwith, diskI/O...These can also impact
  the actual performance.
  3. Asympotic analysis is often related with the size of the input. But in real world
  scenarios, it also need to consider other factors such as the data structure. The
  use of different algorithms should favor corresponding data structures to achieve better
  performance.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  The time complexity of finding a element in a binary search tree is O(logn), n 
  is number of elements in the tree. Therefore, we have log(1000)=3, log(10000)=4, 
  let t1=5seconds, assuming t2 is the unknow time for n=10000. The proportion is 
  t2/t1=log(1000)/log(10000), therefore, t2=t1*(log(1000)/log(10000))=5*(4/3)=6.67seconds.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.
 1. The operation may ignored the constants and lower-order terms, this could have 
 large impact than expect.
 2. The hardware constraints. For example, if the tree with 10000 elements takes more 
 memory than is available in RAM, it could slow down the operations.
 3. The binary tree is unbalanced, leading to a linear growth of the time. (the worst-case)
Add your answers to this markdown file.


