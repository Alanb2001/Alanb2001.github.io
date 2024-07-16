---
layout: page
title: Real-time destruction
description: Unreal engine system
img: assets/img/3P1.JPG
importance: 3
category:
related_publications:
---

This was made as my final year project for my Masters course. I used this as an opportunity to learn how to use Unreal Engine. I only used the C++ side of the engine, and I stayed away from using any plugins such as Chaos Destruction.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3P2.JPG" title="A fracture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image showcases a cube that has fractured
</div>

The way the system works is that it uses Delaunay triangulation to generate the sites of the fracture, and that is then passed on to the Voronoi diagram to use the sites to create the fracture for the shape that is applied to it. In my example, I used a primitive cube, but this should work on any convex shape. The only issue with this system is that since I was also learning how to use Unreal at the same time, I bit off more than I could chew, so unfortunately, the fracture doesn’t happen every single time, and when it does happen, it creates the same shape multiple times. During this project, I learned a lot about unreal and real-time destruction, and I feel like with what I know now, I could make this project a lot better.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/video/Fracturing.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>