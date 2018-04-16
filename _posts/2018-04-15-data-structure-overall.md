---
layout: post
mathjax: true
title: Data Structure Overall(Unfinished)
description: the abstract of all data structures, including complexities, pros, cons, ...
categories: [data_structure]
tags: []
redirect_from:
  - /2018/04/15/
---

* kramdown table of contents
{:toc .toc}

---

# Complexity

There is a great blogger collecting and resorting the complexities of all these common data structures and sorting algorithms. Thanks for his great work.

![Computational Complexity Comparison]({{https://qwe98734.github.io}}/assets/images/screenshots/computational_complexity_comparison.png)

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
		<td align="left"><strong>Stack</strong></td>
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
		<td align="left"><strong>Singly-Linked List</strong></td>
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
		<td align="left"><strong>Skip List</strong></td>
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
		<td align="left"><strong>Binary Search Tree</strong></td>
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
		<td align="left"><strong>B-Tree</strong></td>
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
		<td align="left"><strong>Splay Tree</strong></td>
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
		<td align="left"><strong>KD Tree</strong></td>
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

Among above data structures, the worst space complexities of all are O(n), except the Skip List is O(n log n).

## Array Sorting Algorithms

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

# Reference

[Big-O Cheat Sheet](http://bigocheatsheet.com/), Eric Rowell
