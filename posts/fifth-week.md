---
title: Week 5
published_at: 2025-04-00
snippet: Documentation of My Introduction to Coding!
disable_html_sanitization: true
allow_math: true
---

<script src="./p5.js"></script>

<canvas id="assignment1"></canvas>

<script>
    const cnv = document.getElementById ("assignment1")
    const w = cnv.parentNode.scrollWidth
    const h = w * 9 / 16

    function setup () {
        createCanvas (w, h, P2D, cnv)
    }

    function draw () {
        background (`turquoise`)
        console.log (frameCount)
    }
</script>

---
# Homework 5a


1. Choose a specific work from a post-digital artist and describe it, referring to Florian Cramer's essay What is Post-Digital? to justify why you think this artist classifies as post-digital.

## Matt Kane (@mattkaneartist)

![matt kane art](Pictures/matt.png)

**"Gazers"**-  An artful interpretation of the moon phases that utilises cool colours and implements a hazy glitch effect, in which overlays the moon encased in a lattice box. 

- According to Florian Cramer's 'What is post-digital' essay, she defines it as the "messy state of media, arts and design after their digitisation" and I believe that Matt Kane is a perfect example as a post-digital artist. This artist's produces all his generative artworks digitally, using p5.js to create the glitch effect. I've noticed that the artist tends to put the hashtag of #cryptoart or #nftart which reflects a shift transcending the analog era of art.


2. what technology are they using to produce their work? 

- P5.js 
- Javascript 

Hypothetically, if they were using javascript, what APIs & libraries could they use?
- Web Animations API
- P5js
- PixiJS


3. use RiTa.jsLinks to an external site. to generate a post-digital poem responding to the work in your blog.