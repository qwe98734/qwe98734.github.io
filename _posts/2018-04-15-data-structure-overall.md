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

<style>
tr,td {
	padding: 3px 5px;	
}
</style>
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
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left"><strong>Stack</strong></td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Queue</strong></td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left"><strong>Singly-Linked List</strong></td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Doubly-Linked List</strong></td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">Θ(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">O(1)</td>
	</tr>
	<tr align="center">
		<td align="left"><strong>Skip List</strong></td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Hash Table</strong></td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #00b300; border: 1px solid black;">Θ(1)</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left"><strong>Binary Search Tree</strong></td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Cartesian Tree</strong></td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
	</tr>
	<tr align="center">
		<td align="left"><strong>B-Tree</strong></td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>Red-Black Tree</strong></td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left"><strong>Splay Tree</strong></td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #eaeaea; border: 1px solid black;">N/A</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left" style="background-color: #ffffff; border: 1px solid black;"><strong>AVL Tree</strong></td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">O(log n)</td>
	</tr>
	<tr align="center">
		<td align="left"><strong>KD Tree</strong></td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #00ff00; border: 1px solid black;">Θ(log n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
		<td style="background-color: #f8fd20; border: 1px solid black;">O(n)</td>
	</tr>
</table>

Among above data structures, the worst space complexities of all are O(n), except the Skip List is O(n log n).

# Reference

[Big-O Cheat Sheet](http://bigocheatsheet.com/), Eric Rowell
