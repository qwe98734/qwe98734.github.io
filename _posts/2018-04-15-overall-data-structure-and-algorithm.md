---
layout: post
mathjax: true
title: Overall Data Structure & Algorithm(Unfinished)
description: the abstract of all data structures, including complexities, pros, cons, ...
categories: [data_structure, algorithm]
tags: [time_complexity]
redirect_from:
  - /2018/04/15/
---

* kramdown table of contents
{:toc .toc}

---

# Complexity

There is a great blogger collecting and resorting the complexities of all these common data structures and sorting algorithms. 
Thanks for his great work and wikipedia.


## Computational Complexity Comparison

Graphs of functions commonly used in the analysis of algorithms, showing the number of operations N versus input size n for each function.

![Computational Complexity Comparison](/assets/images/screenshots/computational_complexity_comparison.png)


## Common Data Strucutre Operations

<table>
 	<tr>
		<td style="background-color: #eaeaea; border: 1px solid black;">Data Structure</td>
		<td colspan="8" style="background-color: #eaeaea; border: 1px solid black;">Time Complexity</td>
	</tr>
	<tr>
		<td style="border: 1px solid black;"></td>
		<td colspan="4" style="border: 1px solid black;">Average</td>
		<td colspan="4" style="border: 1px solid black;">Worst</td>
	</tr>
	<tr>
		<td style="background-color: #eaeaea; border: 1px solid black;"></td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Access</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Search</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Insertion</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Deletion</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Access</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Search</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Insertion</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Deletion</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Array</strong></td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong><a href="/blog/2018/04/13/heap/#heading-binary-heap">Binary Heap</a></strong></td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Stack</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Queue</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Singly-Linked List</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Doubly-Linked List</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Skip List</strong></td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Hash Table</strong></td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Binary Search Tree</strong></td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Cartesian Tree</strong></td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>B-Tree</strong></td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Red-Black Tree</strong></td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Splay Tree</strong></td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>AVL Tree</strong></td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>KD Tree</strong></td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
</table>

Note1: among above data structures, the worst space complexities of all are O(n), except the Skip List is O(n log n).

Note2: The "Access" is differed from "Search" and should point to the complexity of accessing a specific element. Take Three examples, first of all, Binary Heap is array-based, so it can access an element by index at O(1) time as same as Array. Secondly, Binary Search Tree(BST) does not have an index system, it needs to traverse through many children to access a specific element at Θ(log n) time, but O(n) time if sorted elements are inserted into an empty BST. Thirdly, Hash Table cannot access an element without a key, so the author defines N/A for accessing a spcific element, but Θ(1) time for search if we have already known the key.


## Common Array Sorting Algorithms

<table>
 	<tr>
		<td style="background-color: #eaeaea; border: 1px solid black;">Algorithm</td>
		<td colspan="3" style="background-color: #eaeaea; border: 1px solid black;">Time Complexity</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">Space Complexity</td>
	</tr>
	<tr>
		<td style="border: 1px solid black;"></td>
		<td style="border: 1px solid black;">Best</td>
		<td style="border: 1px solid black;">Average</td>
		<td style="border: 1px solid black;">Worst</td>
		<td style="border: 1px solid black;">Worst</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Quicksort</strong></td>
		<td style="background-color: #efb28c; border: 1px solid black;">Ω(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">Θ(n log n)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">O(n^2)</td>
		<td style="background-color: #acba9d; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Mergesort</strong></td>
		<td style="background-color: #efb28c; border: 1px solid black;">Ω(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">Θ(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">O(n log n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Timsort</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Ω(n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">Θ(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">O(n log n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Heapsort</strong></td>
		<td style="background-color: #efb28c; border: 1px solid black;">Ω(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">Θ(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">O(n log n)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Bubble Sort</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Ω(n)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">Θ(n^2)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">O(n^2)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Insertion Sort</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Ω(n)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">Θ(n^2)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">O(n^2)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Selection Sort</strong></td>
		<td style="background-color: #e8837e; border: 1px solid black;">Ω(n^2)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">Θ(n^2)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">O(n^2)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Tree Sort</strong></td>
		<td style="background-color: #efb28c; border: 1px solid black;">Ω(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">Θ(n log n)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">O(n^2)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Shell Sort</strong></td>
		<td style="background-color: #efb28c; border: 1px solid black;">Ω(n log n)</td>	
		<td style="background-color: #e8837e; border: 1px solid black;">Θ(n(log n)^2)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">O(n(log n)^2)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Bucket Sort</strong></td>
		<td style="background-color: #749d9b; border: 1px solid black;">Ω(n+k)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(n+k)</td>
		<td style="background-color: #e8837e; border: 1px solid black;">O(n^2)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Radix Sort</strong></td>
		<td style="background-color: #749d9b; border: 1px solid black;">Ω(nk)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(nk)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(nk)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n+k)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Counting Sort</strong></td>
		<td style="background-color: #749d9b; border: 1px solid black;">Ω(n+k)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">Θ(n+k)</td>
		<td style="background-color: #749d9b; border: 1px solid black;">O(n+k)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(k)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Cubesort</strong></td>
		<td style="background-color: #eed19c; border: 1px solid black;">Ω(n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">Θ(n log n)</td>
		<td style="background-color: #efb28c; border: 1px solid black;">O(n log n)</td>
		<td style="background-color: #eed19c; border: 1px solid black;">O(n)</td>
	</tr>
</table>

---

# Reference

[Big-O Cheat Sheet](http://bigocheatsheet.com/), Eric Rowell

[Computational Complexity Comparison Chart](https://en.wikipedia.org/wiki/Time_complexity), Wikipedia

[Data structure - Big O of access and indexing. What do they really mean?](https://stackoverflow.com/questions/39937035/data-structure-big-o-of-access-and-indexing-what-do-they-really-mean?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa), stackoverflow