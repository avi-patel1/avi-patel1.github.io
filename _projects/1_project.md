---
layout: page
title: project 1
description: with background image
img: assets/img/transmission.jpg
importance: 1
category: work
related_publications: true
---

The ME/EE/CS 133a course is the first in the core robotics sequence at Caltech focusing on kinematics and dynamics of robotic systems. 
For our final project, we evaluated the performance of the Boston Dynamics Atlas robot cutting with the right hand and reaching 
to grab an item on a neighboring shelf with the left. We approached this problem in two ways: First, we defined the cutting motion of the 
right arm as the primary task and the left hand as the secondary task. Second, we defined both the right 
and left hand tasks as primary tasks. We described our results including the tradeoffs between both approaches in our final report and video.

 <!-- <a href="/files/ME133a_FinalProject.pdf" target="_blank">Final Report</a>,
<a href="https://github.com/avi-patel1/ME133a" target="_blank">Github</a> -->

<video width="100%" controls>
    <source src="/assets/img/133a_final.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

<iframe style="width:100%; height:500px;" src="https://www.youtube.com/embed/2wi1nkayAvE"></iframe>

<details>
<summary><b> Classic Manipulators, Kinematics, Dynamics - CS/EE/ME 133a </b>
    </summary>
    <p>
        <p> </p>
        <p>
        The ME/EE/CS 133a course is the first in the core robotics sequence at Caltech focusing on kinematics and dynamics of robotic systems. 
        For our final project, we evaluated the performance of the Boston Dynamics Atlas robot cutting with the right hand and reaching 
        to grab an item on a neighboring shelf with the left. We approached this problem in two ways: First, we defined the cutting motion of the 
        right arm as the primary task and the left hand as the secondary task. Second, we defined both the right 
        and left hand tasks as primary tasks. We described our results including the tradeoffs between both approaches 
        in our final report and video.
        </p>
</details>

Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}