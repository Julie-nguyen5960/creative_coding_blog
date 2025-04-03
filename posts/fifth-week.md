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
