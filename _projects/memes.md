---
layout: page
title: Memes
description: A repertoire for the finest math/CS related memes I harvested
img: assets/img/meme_5.png
importance: 1
category: Blog
---

<head>
   <style>
       .center-container {
    display: flex;
    justify-content: center;  /* Horizontally center */
    align-items: center;      /* Vertically center */
    height: 100vh;            /* Use 100% of the viewport height */
}

.centered-image {
    max-width: 100%;          /* Ensure the image doesn't exceed its container */
}
   </style>
</head>


<div class="center-container">
    <img src="{% if site.baseurl %}{{ site.baseurl }}{% endif %}/assets/img/meme_1.png" alt="Your Image Description" class="centered-image">
</div>
