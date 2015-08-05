---
layout: post
title: Hack Reactor pre course prep and my first Hackathon
category: article
tags:
 - hack reactor
 - coding
 - archives
---

<!--![Image description](/images/config.png)-->
  
  <article class = post>
    <p>Yesterday, I received access to all the prep work to HR, and it is a LOT of stuff. The prep work is structured from Low to High complexity. Starting from basic JS to recursion.</p>
    <p>I feel like I need to come up with a solid schedule, since all the prep work has deadlines, and they are Mandatory</p>
    <h3>Plan of attack!</h3>
    <p>DON't LOOK AT SECTION II AND III, FOCUS ON I</p>
    <p>Go back to the basics, start from the beginning, focus on fundamentals in section I. Since I am looking at 11+ hours a day, once I start the program, I need to ramp up slowly to putting that many hours sitting in front of my screen. so I plan to start with six, and slowly pace up to 11, incrementing 1++ hour each day</p>
    <p>I also want to keep learning Flask, so I plan to devote a few hours working on my Flask side project. Lets see how that works out. Last weekend I attended my first ever Hackathon, I built this awesome web app with a bunch of ladies from <a href="https://www.girldevelopit.com/">Girl Develop it</a>. The app is called <a href="http://neohack-platypus-renegades.herokuapp.com/">What's cool on NPR</a>. It filters programs from NPR based on users likes. We built this using the NPR API, and for backend we used <a href="https://www.firebase.com/docs/web/">Firebase's web platform</a>, which made it super easy to read and write data since it already comes with the Node.js API. This was my first time using a NoSQL database to build somethng from scratch, I found it to be super easy and very intutive. All the data is stored as a JSON tree.</p>
<p>{ <br>
  "users": {<br>
    "mchen": {<br>
      "friends": { "brinchen": true },<br>
      "name": "Mary Chen",<br>
      // our child node appears in the existing JSON tree<br>
      "widgets": { "one": true, "three": true }<br>
    },<br>
    "brinchen": { ... },<br>
    "hmadi": { ... }<br>
  }<br>
}<br>
</p>

<p>Firebase also has a Dashboard, which makes for a nice visual in the way data is represented. To access the child node you just reference it with the parent node, very similar to the DOM API. I really like the idea of data storage in the form of trees, this eliminates the need for tables and the tedious SQL queries, my only issue would be when you have lots of data and the nodes and sub nodes increase, but I am guessing you can create seperate JSON objects, and link them in some way to avoid a unmanageable tree.</p>
   

