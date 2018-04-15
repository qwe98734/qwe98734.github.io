---
layout: post
mathjax: true
title: Data Structure Overall(Unfinished)
description: the abstract of all data structures, including complexities, pros, cons, ...
categories: [data structure]
tags: []
redirect_from:
  - /2018/04/15/
---

* kramdown table of contents
{:toc .toc}

---

# Complexity

There is a great blogger collecting and resorting the complexities of all these common data structures and sorting algorithms. Thanks for his great work.

<table class="ss3">
 	<tr>
		<td>Data Structure</td>
		<td colspan="8">Time Complexity</td>
	</tr>
	<tr>
		<td></td>
		<td colspan="4">Average</td>
		<td colspan="4">Worst</td>
	</tr>
	<tr>
		<td></td>
		<td>Access</td>
		<td>Search</td>
		<td>Insertion</td>
		<td>Deletion</td>
		<td>Access</td>
		<td>Search</td>
		<td>Insertion</td>
		<td>Deletion</td>
	</tr>
	<tr align="center">
		<td align="left">Array</td>
		<td>Θ(1)</td>
		<td>Θ(n)</td>
		<td>Θ(n)</td>
		<td>Θ(n)</td>
		<td>O(1)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
	</tr>
	<tr align="center">
		<td align="left">Stack</td>
		<td>Θ(n)</td>
		<td>Θ(n)</td>
		<td>Θ(1)</td>
		<td>Θ(1)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(1)</td>
		<td>O(1)</td>
	</tr>
	<tr align="center">
		<td align="left">Queue</td>
		<td>Θ(n)</td>
		<td>Θ(n)</td>
		<td>Θ(1)</td>
		<td>Θ(1)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(1)</td>
		<td>O(1)</td>
	</tr>
	<tr align="center">
		<td align="left">Singly-Linked List</td>
		<td>Θ(n)</td>
		<td>Θ(n)</td>
		<td>Θ(1)</td>
		<td>Θ(1)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(1)</td>
		<td>O(1)</td>
	</tr>
	<tr align="center">
		<td align="left">Doubly-Linked List</td>
		<td>Θ(n)</td>
		<td>Θ(n)</td>
		<td>Θ(1)</td>
		<td>Θ(1)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(1)</td>
		<td>O(1)</td>
	</tr>
	<tr align="center">
		<td align="left">Skip List</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
	</tr>
	<tr align="center">
		<td align="left">Hash Table</td>
		<td>N/A</td>
		<td>Θ(1)</td>
		<td>Θ(1)</td>
		<td>Θ(1)</td>
		<td>N/A</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
	</tr>
	<tr align="center">
		<td align="left">Binary Search Tree</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
	</tr>
	<tr align="center">
		<td align="left">Cartesian Tree</td>
		<td>N/A</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>N/A</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
	</tr>
	<tr align="center">
		<td align="left">B-Tree</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left">Red-Black Tree</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left">Splay Tree</td>
		<td>N/A</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>N/A</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left">AVL Tree</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
		<td>O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left">KD Tree</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>Θ(log n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
		<td>O(n)</td>
	</tr>
</table>


# Reference

[Big-O Cheat Sheet](http://bigocheatsheet.com/), Eric Rowell
