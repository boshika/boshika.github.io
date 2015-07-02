---
layout: post
title: Hack Reactor pre course prep and my first Hackathon
content: 
---

<!--![Image description](/images/config.png)-->
  
  <article class = post>
    <h1>Received the pre prep work to HR, and this is going to be  fun</h1>
    <p>Yesterday, I received access to all the prep work to HR, and it is a LOT of stuff. The prep work is structured from Low to High complexity. Starting from basic JS to recursion.</p>
    <p>I feel like I need to come up with a solid schedule, since all the prep work has deadlines, and they are Mandatory</p>
    <h3>PLan of attack!</h3>
    <p>DON't LOOK AT SECTION II AND III, FOCUS ON I</p>
    <p>Go back to the basics, start from the beginning, focus on fundamnetals in section I. Since I am looking at 11+ hours a day once I start the program, I need to ramp up slowly to putting that many hours sitting in front of my screen. so I plan to start with six, and slowly pace up to 11, incrementing 1++ hour each day</p>
    <p>I also want to keep learning Flask, so I plan to devote a few hourse working on my Flask side project. Lets see how that works out. Last weekend I attend my first ever Hackathon, I built this awesome web app with a bunch of ladies from <a href="https://www.girldevelopit.com/">Girl Develop it</a>. The app is called <a href="http://neohack-platypus-renegades.herokuapp.com/">What's cool on NPR</a>. It filters programs from NPR based on users likes. We built this using the NPR API, and for backend we used <a href="">Firebase's web platform</a>, which made it super easy to read and write data since it already comes with the Node.js API. This was my first time using a NoSQL database to build somethng from scratch, I found it to be super easy and very intutive. All the data is stored as a JSON tree.
{
  "users": {
    "mchen": {
      "friends": { "brinchen": true },
      "name": "Mary Chen",
      // our child node appears in the existing JSON tree
      "widgets": { "one": true, "three": true }
    },
    "brinchen": { ... },
    "hmadi": { ... }
  }
}
</p>

<p>Firebase also has a Dashboard, which makes for a nice visual in th way data is represnted. To acess the child node you just reference it witht he parent node, very similar to the DOM API. I really like the idea of data storage in the form of trees, this elimiantes the whole need for tables and the tedious SQL queries, my only issue would be when you have lots of data and the nodes and sub nodes increase, but I am guessing you can create seperate JSON objects, and link them in some way to avoid a unmanageable tree</p>
   

