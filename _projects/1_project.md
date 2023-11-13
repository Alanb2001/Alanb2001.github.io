---
layout: page
title: Procedural cave generation
description: Unity engine system
img: assets/img/1P1.JPG
importance: 1
category:
related_publications:
---

This was made as a part of my final year project, I used C# and the Unity game engine. The system uses Perlin noise to create the cave system. The idea behind it was designed
to be used by people to make caves for there games or to just play around with.   

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1P2.JPG" title="A cave chunk" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image showcases a bit of the cave generated.
</div>

The way the system works is that it will generate chunks of the cave based on a seed given to the Perlin noise generator and this
dictates how the cave will look like. It is infinitely generated but there is a fixed size of chunks that get loaded in at one time to
avoid lag, once a chunk gets deloaded its coordinates get remembered by the system so if you return to the same spot it'll be the same
chunk that was seen previously.   

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/video/CaveGen.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>