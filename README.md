# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asympotic analysis ignored the constant factor and lower-order terms, in the
  real world practical scenarios with finite input, these factos can impact the
  performance significantly.
  2. Asympotic analysis is a theoretical model, it does not account for the real-world
  hardware, such as CP cache size, memory bandwith, diskI/O...These can also impact
  the actual performance.
  3. Asympotic analysis assumes worst-case, best-case, or average-case scenarios, based 
  on a theoretical model of data distribution, but in real-world situation, the distribution
  of the data could be varied(skewed or repetiyive data), it can casue an unexpected performance.
  For example, the unbalanced binary search tree.

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
 1. The way how the BST is implemented could be problematic when the input size gets larger.
  For example, how nodes are created, managed and traversed.
 2. The hardware constraints. For example, if the tree with 10000 elements takes more 
  memory than is available in RAM, it could slow down the operations.
 3. The binary tree is unbalanced, the structure becomes to a linked list. For example, if
  searching for a value near the bottom of that skewed tree, every single node need to be checked,
  this could increase the time linearly with the number of elements.

“I certify that I have listed all sources used to complete this exercise,
 including the use of any Large Language Models. 
 All of the work is my own, except where stated otherwise. 
 I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, 
 charges may be filed against me without prior notice.” --Doris Yan


