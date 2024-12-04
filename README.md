[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  Asympotic analysis bases an algorithms performace largly on input sizes, and how an algorithm opperates based on these input sizes. Actual runtime can be affected by factors that are not accounted for when an algorithm runs. A few of these factors include:
  1) Asympotic analysis looks strictly at the opperations that are being excecuted on an input, and how long they take in general. Software and hardware can be a factor that gets overlooked in this, as some machines may result in diffent complexities than others.
  2) Asympotic analysis looks at a sort of "whole picture" when deciding how long an algorithm takes to run, and ignores opperations that take constant time to complete. This constant time can add up and take longer than expected when working with large input sizes, resulting in a longer runtime than a $\Theta$ representation could suggest.
  3) Asympotic analysis also ignores lower order terms that arise in in algorithm. If an algorithm has a complexity of $O(n^2 + n^4), it is simplified to $O(n^4)$, however the $n^2$ can be rather large with large inputs, yeilding longer runtime results.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

The Asympotic analysis of a binary search tree is $O(log(n))$, for 1,000 elements we have log(1000) = 

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

Theory vs practice differs in the case of assumptions, assuming a time complexity consists of hardware and operating systems, as well as an assumption of input, which cause fluxuation in actual real world execution. These factors can alter real world run times. 

10,000 elements would take roughly 13.3 seconds, $(4(log2(10) = 13.3)$

Factors such as: the data structure not fitting entirely in the cache, an unbalanced data structure such as a tree being skewed to one side, and the actual algorithm implementation can cause differences in expected time complexity and actual time taken to run could be a reason that the 10,000 element list would take 100 second to sort.

Help: ChatGPT and Stackoverflow.com
