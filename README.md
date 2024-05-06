[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ZLHpg3lN)
# Quicksort

Implement an iterative (no recursive calls) version of quicksort. Use the
template I've provided in `code.js`. Test your new function; I've provided some
basic testing code that uses [jsverify](https://jsverify.github.io/) in
`code.test.js`.

Hint: To make quicksort iterative, think about the part of the array each
recursive call considers.

## Runtime Analysis

Analyse the time complexity of your implementation and give a $\Theta$ bound for
its worst-case runtime. Add your answer, including your reasoning, to this
markdown file.

The worst case for this would be if the partition function doesn't split the array evenly and picks a bad pivot. If it was already sorted or reverse sorted the partition function splits the array into sub-arrays equal to $n-1$ and 1 and then the last element would
be chosen as the pivot. The theta bound would be $O(n^2)$ because the partition function take $O(n)$ time and needs to be called $n$ times. The first call will go through $n$ elements the the second call would process $n-1$ elements and so on until the last call that would process 1 element. So, $(n*(n+1))/2$ and that's $O(n^2)$




https://www.geeksforgeeks.org/hoares-vs-lomuto-partition-scheme-quicksort/


https://dev.to/henryong92/quick-sort-14d9


https://github.com/ivandi1980/codechef/blob/f5a4007a52caf274050ebd96196561d1736c4088/quick_sort.js
