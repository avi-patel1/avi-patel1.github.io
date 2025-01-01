---
layout: page
title: Ghost Path Planner for Pac-Man
description: Planning, Localization and Navigation - CS/EE/ME 133b 
img: assets/img/133b_final_gif.gif
importance: 2
category: work
giscus_comments: false
---

The ME/EE/CS 133a course is the second in the core robotics sequence at Caltech focusing on path planning, localization and navigation. For our final project, we developed various planning algorithms for the ghosts to chase and capture Pac-Man. In the first approach, we sequentially planned each ghost's path using A*. In the second approach, we create a region planner which using breadth-first search to identify potential locations where Pac-Man could arrive for the ghosts to target. In the last approach, we create a multi-dimensional planner where each node in our graph contains the coordinates of all ghosts. We evaluated the performance of each approach and examined the trade-offs between them in our final report and video.

<p>Links to project: 
    <a href="/assets/pdf/ME133b_FinalProject.pdf" target="_blank">Final Report</a>,
    <a href="https://github.com/avi-patel1/ME133b" target="_blank">Github</a>
</p>  

<video width="100%" controls>
    <source src="/assets/video/ME133b_finalVideo.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>