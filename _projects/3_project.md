---
layout: page
title: Mobile Robot
description: Experimental Robotics - CS/EE/ME 129
img: assets/img/129_bot.jpg
# redirect: https://unsplash.com
importance: 3
category: work
---

I built a mobile, line and wall following robot as part of the CS/EE/ME 129 course at Caltech.
The hardware includes three IR sensors for line following, end of road
and intersection detection behaviors, a magnetometer board to measure the orientation 
of the robot and three ultrasonic sensors to detect blockages in front and at the sides 
of the robot.

<img src="/assets/img/129_Bot_rename.png" width="500" height="500" class="align-center"
alt="Diagram">

<p> </p>
For the robot's software, I wrote the autonomous navigation algorithms, UI and mapping. 
At every intersection, there are eight possible headings for the robot to explore. 
Each heading (streets) is denoted by the following status colored on the map shown in the video below:

<ul>
    <li><span style="color:black;"> Black</span>: existence of the street is unknown</li>
    <li> <span style="color:blue;"> Blue</span>: street exists but is unexplored</li>
    <li><span style="color:green;"> Green</span>: street is fully explored (connect to another intersection)</li>
    <li><span style="color:red;"> Red</span>: street has a dead end</li>
</ul>
I implemented Dijkstra's algorithm to find the optimal path to a goal node set by the user. 
If the node is not on the current map, I implemented Dijkstra to the nearest nodes with unexplored headings
while also exploring the map in the direction of the goal.
Blockages are denoted by a red X on the map in the video below. The robot is able to replan around static blockages
along with perform a panic u-turn on moving blockages. 

Below is a demonstration of the robot where we run directed explore to some goal node. 

<video width="700" height="500" controls>
    <source src="/assets/video/129Demo.mp4" type="video/mp4"></video>
