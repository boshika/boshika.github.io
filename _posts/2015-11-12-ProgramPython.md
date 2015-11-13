---
layout: post
title: Elegance of Python
category: article
tags:
 - coding
 - python
 - archives
---
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Beauty in Python</title>
</head>
<body>
<h1>Do you see?</h1>
<h3>Read the code below</h3>
<script src="https://gist.github.com/boshika/dc6e62eb34f98d6ca09d.js"></script>
<p>It is a simple program. It accepts a file, opens it , reads the file line by line. It specifcally looks for lines that start with From, but also ignores files that have From w/ :. We count all the lines with From, then we create a list by spiliting each line using the single-quote delimeter. This was we create a list, we then only print the second value in the list, and also print the total count in the end. </p>
<p>So, here the thing to not eis how verbose the program. Here in lies the beauty of Python. Instead of using braces to block scoping, Python utilizes indentation, incredibily simple; Start a loop(for, if..else, while etc etc), put a ":" , next line indent, when done writing the loop de-indent, done!</p>
<p>If this was not easy enough, you have to atleast admire the fluency of the if statement, it is like writing a sentence in English.</p>
<h4>Here is another small program</h4>
<script src="https://gist.github.com/boshika/a7638ad20c50cd2f1427.js"></script>
<p>Very similar to the above example, difference is we are comparing two lists. Look at the first for statement "for val in line", basically we have alist of all lines, and for each value, we are comapring it to the values in the second list, and if they both have same value, "continue", else add teh value using append()[similar to push()] to the second list</p>
<p>Simple!</p>
<p>Next blog post about functions and OOP in Python</p>
</body>
</html>
