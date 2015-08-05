---
layout: post
title: Hack Reactor pre-course prep lessons learnt--Lesson 1
category: article
tags:
- hack reactor
- coding
- challenges
- 2015
---
<!--<!DOCTYPE html>-->
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Pre-course lessons learnt</title>
</head>
<body>
<h3>Finished HR pre-course prep!!!!!!</h3>
<p>
  It was roughly a month ago that I recieved the HR pre-course prep work..I procrastinated for a week or so before I started the prep work. It took approximately 2 weeks to finish. Without giving away too much, here are a few lessons/things learnt while finishing the prep work.
</p>
<h4>Lesson 1: UnderBar</h4>
<p>
  The first big assignment was to re-implement some of the most useful, and commonly used Underbar functions. Moving from more easy functions to some really hard ones. The first half of the assignemnt was easy, the challenges started showing up in the scond half where I had to re-implement some really interesting methods.
<br>Some really neat things I picked up during these re-implementations were the use of <bold>"arguments object"</bold>, and <bold>"Array.prototype.slice.call"</bold>
</p>
<p>
  Arguments object within JavaScript, is a local variable that is availbale within all functions. This is really useful when you need to access functions original arguments for some further manupulation. Say you have these objects { x: 'x' }, { a: 'a', x: 2 }, { a: 1 }, and a function called myfunc. You pass these objects as arguments to myobj function()</p>
<p><script src="https://gist.github.com/boshika/0d99be851e6a52fc32dd.js"></script></p>
<p>myobj({ x: 'x' }, { a: 'a', x: 2 }, { a: 1 })<br>
  Result:<br>
   Object {x: "x"} <br>
   Object {a: "a", x: 2} <br>
   Object {a: 1}<br>
</p>
<p>As you can see from the above example, all you do is use arguments[0], arguments[1]...and so on to access the inside objects. arguments object stores the original arguments passed in a function in an array like object, which acts similar to an array, where each argumment is stored at an index starting at index 0</p>
<p>One important thing to note is that arguments object is NOT an array, it does behave like an array when it comes to indexing the function arguments, and can also return the arguments length, but this is where the similarities end...you cannot push/pop/shift/unshift using arguments object...</p>
<p>This is where Array.prototype.slice.call() comes in handy, you can use this to convert these arguments objects into proper arrays</p>
<p><script src="https://gist.github.com/boshika/9d2b58ba19c35c1be0f2.js"></script>
</p>
<p> 
  This will return a prototype array of the arguments which looks like this [Object, Object, Object], and along with it a list of all array methods that can be used on the prototype.
</p>
<p>More Lessons learnt in the next post...</p>
</body>
</html>
