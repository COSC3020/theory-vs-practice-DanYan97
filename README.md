# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
  1.Asympotic analysis ignored the constant factor and lower-order terms, in the
  real world practical scenarios with finite input, these factos can impact the
  performance significantly.
  2.Asympotic analysis is a theoretical model, it does not account for the real-world
  hardware, such as CP cache size, memory bandwith, diskI/O...These can also impact
  the actual performance.
  3.Asympotic analysis is often related with the size of the input. But in real world
  scenarios, it also need to consider other factors, such as the distribution of the input,
  data structure 

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.


