---
title: Week 1
published_at: 2025-03-07
snippet: Documentation of My Introduction to Coding!
disable_html_sanitization: true
allow_math: true
---

# Homework task pt. 1

This is my first time touching code, so I find myself struggling to understand anything and becoming overwhelmed with this new language. Upon looking at the homework tasks, I found it jarring to look at all the lines of code for this [sketch](https://editor.p5js.org/capogreco/sketches/-B11g3Uth). So rather than attempting to create the grid, I tried dissecting the code for this sketch through the help of my friend and my little brother who are more experienced in coding.

My friend hopped onto voice chat to explain to me about how the code for the 'For Loop' works and what it is doing. She managed to explain how some strings worked and how the code creates loops.

![friend explaining](Pictures/explain.jfif)

## Rafael Rozendaal's work: Blocks

I am completely clueless how Rozendaal was able to attain such effect but I'm guessing that he had to code for the colour change of the two rectangles that expand and shrink on screen. The colour change of the background probably have to allign with the two rectangles' frameCount to ensure they change colour at the same time. Then one of the rectangles have to expand whilst the other starts to disappear at a certain point of the canvas.

(insert diagram)

**list of concepts to replicate the work**

- The drawing function prompting to draw a rectangle: rect ()
- To set a range of colours to appear, either using RGB or HSB: Fill ()
- Track the number of frames drawn: frameCount
- possibly using the mode RADIUS instead of CENTER: rectMode (RADIUS).

**List of resources to help learn those concepts**

- The [p5js](https://p5js.org/reference/) website for references
- ChatGPT- to understand concepts of coding
- Tutorials on Youtube eg. The Coding Train

# Homework task 2

As for this class activity, I wasn't able to participate in group discussions due to stomach issues, hence why I came late to class. First thing I got started on was asking for help in fixing my issue with the 'deno task start' command not working. However, these issues have been fixed and now I am able to publish my blog onto the browser!

In order to test out my theory, I had to test out some of the concepts that I have listed in the previous homework task. I did not test all of my proposed concepts but I did my best to replicate how the squares expand on screen in the first few frames.I tried to implement code that was easy for me to intepret.

## My attempt:

<iframe id="attempt_block" src="https://editor.p5js.org/Julie-nguyen5960/full/JVNz4BlQB"></iframe>

<script type="module">

    const iframe  = document.getElementById (`attempt_block`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 50 / 50 + 42
