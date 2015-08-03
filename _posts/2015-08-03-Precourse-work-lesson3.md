---
layout: post
title: Hack Reactor pre-course prep lessons learnt--Lesson 3
content: 
---

<!-- <!DOCTYPE html> -->

<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Pre-course lessons learnt</title>
</head>
<body>
	<h4>Lesson 3: Dreaded Recursion</h4>
	<p>
	 Last year in graduate school, I took a class In Data Structures, and Algorithms in Java, and Yes, of course we learnt the "dreaded Recursion", at that time, it all went over my head...so when I saw Recursion assignment on the HR pre-course list, needless to say I had a minor nervous breakdown, and for good reasons
	</p>
	<h4>Here is how I learnt the dreaded recursion at grad school</h4>
	<ul>
	  <li>A general case expressed in terms of a simpler version of itself</li>
	  <li>A stopping case--trivial, non-recursive</li>
	  <li>Application of the general case leading to a stopping case e.g. 5!= 6!/6</li>
		<ul>
			<li>a numerically correct result</li>
			<li>Leads aay from stopping case</li>
		</ul>
	  </li>
	</ul>
	<h3>Fibonacci Example</h3>
	<script src="https://gist.github.com/boshika/de97725a64bdd3ff436f.js"></script>
	<p>...and a lot of blahh...blahhh..Towers of Hanoi...blah...blah...This is what I learnt</p>
	<h4>Here is what i learnt while completing the HR Recursion prep work</h4>
	<p>
	 <strong>recursion is calling a function on itself.</strong>
	 key features of recursion are: base case: this is a statement, usually within a conditional clause like if, that stops the recursion. If you don't have a base case, the recursion will go on infinitely and your program will crash. Crash = bad.
	</p>
	<p>
	 The second is a recursive case: this is the statement where the recursion actually happens: where the recursive function is called on itself.
	</p>
	<script src="https://gist.github.com/boshika/b333c2b517e12724fb19.js"></script>
	<h5>Fibonaccir Beanstalk</h5>
	<p>
	 What is Fibocacci sequence: Fibonacci sequence, whereby each element in the sequence is equal to the sum of the two previous elements: 1, 1, 2, 3, 5, 8, 13, 21...
	</p>
	<h4>Iplementation of Fibonacci sequence</h4>
	<script src="https://gist.github.com/boshika/0c803c0641a06311fd74.js"></script>
	<p>
	 This was from the Codeacademy Recursion tutorial...half-way point through the course, and I understood more about recursion then I did in my entire graduate class
	</p>
	<p>
	 Moral of the story---if something can be explained in simpler terms, explain it in simpler terms...it is not <strong>important</strong> that you understand the technical jargon, it is more iportant to understand the idea behind it!
	</p>
</body>
</html>