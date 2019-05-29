---
title: Creating Math-Based 3D Models
layout: post
tags:
- invention
aggregatelimit: 4
imagecredit: Procedural Recursion by <a href="http://bluevisual.tv/personal/pyramidfractal/">Kevin
  Weber</a>
unlistedtags: programming art 3dprinting math
date: 2018-04-30 00:00:00 +0000
image: "/assets/images/Procedural Recursion.jpg"
unusedtags: ''
---
One of my clients requested a longer form 3-D Printing class that needed a tangible immediate benefit present when participants went to the class. One of the ideas that came up was to use mathematical formulas to create 3-D objects. The goal was to be able to show every day tangible benefits to knowing math and 3D printing and using it in an artistic fashion. <!--excerpt-->

Research was started by looking for math based art examples. One artist in particular that popped up was <a href="https://www.scientificamerican.com/author/hamid-naderi-yeganeh/"> Hamid Naderi Yeganeh </a> and he was featured in Scientific American. His methodology created gorgeous mathematics but getting up to speed to do what he does was a bit outside our target demographic.

Let's bring it back to the priorities of the project:

* Applied math, art, and 3D printing
* Low budget
* Usable on Linux
* K-6 education market
  * Ease of use
  * Accessible
  * Practicable away from the teaching site
  * Quick Feedback

As the target audience has no background in programming I wanted to find a tool that did most of the math-> computer language  heavy lifting as we wanted this class to be done over 6 sessions and teaching how to code was not in the scope of work nor what the end user would want to work with. I kept researching along the lines of graphing math for educators and came across this tool called <a href="https://www.desmos.com/">DESMOS</a> and specifically it's calculator tool.

DESMOS was great, we could use it to make rudimentary math based 2-D drawings using the slope intercept form y=mx+b or quadratic equations or trigonometric functions. We can teach these fundamental tools to make 3-dimensional objects treating the formulas like paintbrushes. It works in parametric or polar forms and you can have both mathematical models projected upon one another. The only "problem" we had was that it would not generate a CAD friendly format. Luckily, the software had the ability to export an image with just the function without the axes or markings and I had experience turning raster images into svgs via a litle program called inkscape.

For all 3D manipulation of my client's models, we used the free software suite [Tinkercad](). Tinkercad let’s you import svg files and turn them into simple extrusions. Not only that, There is a featured community tool that allows you to create revolved models using the svg as the profile.

For all of our prints, we used a service called Polar Cloud in conjunction with the client’s local Filterforge Inventor printers.

Now that we have all the tools figured out, we needed to figure out how the curriculum should be staggered to make the most of the six days available to us and the student.

On the first day, the student is introduced to the basic mathematical formulas  without having to make them learn what the math is actually doing. So in DESMOS, basic formulas are presented like

y=0

x=0

y-mx=0

y-e^x=0

y-sin(x)=0

y-tan(x)=0

y-sinh(x)=0

y-tanh(x)=0

y^2+x^2=0

Once the basic formulas are set up, we put some handles on the formulas like the following:

y-b=0 {a<x<c},

x-a=0 {b<y<c},

\(y-(b))-m(x-(a))=0 {f<x<g} {h<y<i},

\(y-(b))^2-m(x-(a))^2=0 {f<x<g} {h<y<i}

The formulas are then used to create a basic 2D drawing,by following these procedures: 

1. Clicking on the gear icon and clicking on the color for each formula, change all the colors to black. 
2. Hide the list by pressing the double left carat button.
3. Click on the wrench icon to hide the grid, X-Axis and Y-Axis.