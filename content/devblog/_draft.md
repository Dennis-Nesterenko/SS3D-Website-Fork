
+++
draft = true
+++

---
layout: post
title:  "00.00 (year.month) : [insert month/quarter] Devblog"
date:   2020-00-05 (year-month-day) 06:30:00 +0100    // The date should be the day the devblog is released and becomes part of the link to the post on the site. Also the website will not post with a future date and time.
description: |
    "Description goes here."
authors: [insert author name]
extra:
  image: /assets/img/art/[insert folder]/[insert wallpaper].png
  image_credit: [insert artist name]
  release: [insert release tag]   // This MUST match the related release tag on GitHub.
aliases: [year/month/day/yearabbreviated.month.html]
---

Cute phrase/quote goes here.

// The devblog is mostly laid out in sections. With the titles of the sections going from large = # (recap section), to medium = ## (content sections), to small = ### (info sections). These are not rules but more like guidelines, take liberty in moving or renaming sections as well as deleting/merging unneeded sections.

// Bold any **names** when referencing someone in a description.

// Linking to internal file:
[Text]({{ site.baseurl }}/[insert folder]/File.format)

// Linking to external file:
[Text](File.Link)

# [Insert Month/Quarter] Recap

[Insert Recap Summary]

## Special

// 'Special' is any content from other categories specifically intended to show first.

[Insert Description]

[Insert Media]

// Avoid gifs if possible and ensure reasonable file size if you do.

// Displaying an image:
{{ image(kind="post", src="assets/img/posts/[insert folder]/Image1.png") }}

// Displaying 2 images horizontally:
<div class='horizontal-2' markdown='1'>
  {{ image(kind="split", src="assets/img/posts/[insert folder]/Image1.png") }}
  {{ image(kind="split", src="assets/img/posts/[insert folder]/Image2.png") }}
</div>

// Displaying 3 images horizontally:
<div class='horizontal-3' markdown='1'>
  {{ image(kind="split", src="assets/img/posts/[insert folder]/Image1.png") }}
  {{ image(kind="split", src="assets/img/posts/[insert folder]/Image2.png") }}
  {{ image(kind="split", src="assets/img/posts/[insert folder]/Image3.png") }}
</div>

// Displaying a slideshow of images (no more than 6 images (mySlides) per page (myRows)):
<div class="slideshow">
  {% include slideshow.html %}
  <div class="mySlides">
    <div class="slide-number">1 / X</div>
    {{ image(kind="split", src="assets/img/posts/[insert folder]/Image1.png") }}
    <div id="description" class="slide-description">[insert description or delete this div]</div>
  </div>
  <div class="myRows">
    <div class="row">
      <div class="column">
        <img class="thumbs cursor" src="{{ get_url(path="/assets/img/posts/[insert folder]/Image1.png) }}" style="width:100%" alt="Image 1" onclick="currentSlide(1)">
      </div>
    </div>
  </div>
</div>   

// Displaying a gif:
{{ image(kind="split", src="assets/img/posts/[insert folder]/gif1.gif") }}

// Displaying a video:
// Removed 'muted' if the video has sound.
// Remove 'controls' and add 'autoplay' and 'loop' if you want it to loop.
<video autoplay="autoplay" muted loop="loop" width="580px" poster="/assets/img/posts/[insert folder]/VideoThumbnail.png">
  <source src="/assets/img/posts/[insert folder]/Video.mp4" type="video/mp4">
</video>

// Displaying 2 videos horizontally
<div id="doublevid"> 
    <video id="vid1" width="285" height="285" poster="/assets/img/posts/[insert folder]/VideoThumbnail.png" autoplay loop muted> 
      <source src="/assets/img/posts/[insert folder]/Video.mp4" type="video/mp4">
    </video>
    <video id="vid2" width="285" height="285" poster="/assets/img/posts/[insert folder]/VideoThumbnail.png.png" autoplay loop muted> 
      <source src="/assets/img/posts/[insert folder]/Video.mp4" type="video/mp4">
    </video>
    <div class="vidclear"></div> 
</div>

## Core-Systems

// 'Systems' is what it sounds like, but I usually change the section name to the name of the system (interaction, atmospherics, tilemaps, chat, etc).

## Fixes

## 3D Assets

## 2D Assets

// '2D' is logos, graphics, decals, etc.

## Sound

// 'Sounds' is sound effects, music, noises, etc.

## Concepts

// 'Concepts' are concept drawings, animations, systems, etc.

## Artwork

// 'Artwork' is artistic wallpapers, animations, etc. (not meant for in-game use).

## Other

// 'Other' is any assets not fit for another section.

### Updates/Notes/Conclusion

// 'Updates' is updates events or changes relating to management, systems, or other logistics.

// 'Notes' is miscellaneous info that may be of interest (e.g. )

// 'Conclusion' is the final wrap-up and goodbye, and include the discord link, as tradition.

Goodbye summary goes here, including our discord link. {{ link(key="discord_url", text="Discord link", path="") }}
