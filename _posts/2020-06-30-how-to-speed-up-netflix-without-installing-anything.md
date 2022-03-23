---
title: How to Speed Up Netflix Without Installing Anything
published: true
description: document.querySelector('video').playbackRate = 2;
tags: tips, productivity, javascript, tutorial
cover_image: https://dev-to-uploads.s3.amazonaws.com/i/0rdte0qgyijpcbzovlmu.png
---

```js
document.querySelector('video').playbackRate = 0.5;

document.querySelector('video').playbackRate = 1.5;

document.querySelector('video').playbackRate = 2.0;

document.querySelector('video').playbackRate = 3.0;
```

I don't want to install anything just to speed up Netflix. If you do, [there are options](https://thedroidguy.com/change-netflix-playback-speed-1119495). For my part, whenever I move to a new computer, I look up this incantation. I'm posting it myself to speed that up next time.

Open your browser's inspection tool to get to the JavaScript console, then enter this line of code with a number corresponding to the speed. `2.0` or `2` is 2x speed. It takes any non-negative number, including numbers between `0` and `1` to slow down the video. (`0` pauses playback.) It also works for any HTML5 video, not just Netflix. The `'video'` string is the default name and extremely common, although the website *can* change it to something else.

The real solution to this problem is Netflix exposing the HTML5 speed controls through their interface, but they are ghouls who refuse to do that. Likewise, there are creeps in Hollywood who insist they have some fictional right to make you watch TV at 1x speed against your will, and they lobby Netflix to prevent this functionality that already exists. They're making choices for you, and they are choosing to waste your life away. Be the lowest-tier cyberpunk you can be and take your time back from these monsters. At least, when you want to.
