---
title: Week 5
published_at: 2025-03-00
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

1. pick a post-digital artist from our discord channel, or from elsewhere on the internet.  Choose a specific work and describe it, referring to Florian Cramer's essay What is Post-Digital? to justify why you think this artist classifies as post-digital.

2. what technology are they using to produce their work? 
- Hypothetically, if they were using javascript, what APIs & libraries could they use?


3. use RiTa.jsLinks to an external site. to generate a post-digital poem responding to the work in your blog.