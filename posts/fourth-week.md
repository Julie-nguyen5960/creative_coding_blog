---
title: Week 4
published_at: 2025-04-07
snippet: Glitch effects
disable_html_sanitization: true
allow_math: true
---

[Read Week 3](/third-week)

[Read Week 5](/fifth-week)

---

# Homework task 4a

### 1. Please use either Canvas API or the p5 online editor to create three example compositions, demonstrating:

**1. high compressibility**

- A sketch that appears more orderly and contains more organised patterns, Make the code more reusable for these objects and compress it into a smaller codes.
<iframe id="pattern" src="https://editor.p5js.org/Julie-nguyen5960/full/CGCNsdsWp"></iframe>

<script type="module">

    const iframe  = document.getElementById (`pattern`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

**2. low compressibility**

- A sketch where most things are out of order and random, which makes the code harder to compress due to the different attributes of each object.

<iframe id="doots" src="https://editor.p5js.org/Julie-nguyen5960/full/_3wweTaEW"></iframe>

<script type="module">

    const iframe  = document.getElementById (`doots`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

_Tutorial from [The Coding Train](https://www.youtube.com/watch?v=nfmV2kuQKwA)_

**3. high effective complexity**

- A sketch where it blends the two, high compressibility and low compressibility. It will contain some structure whilst having some random elements.

<iframe id="high effective" src="https://editor.p5js.org/Julie-nguyen5960/full/gjyAP1-Vh"></iframe>

<script type="module">

    const iframe  = document.getElementById (`high effective`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

_Tutorial from [UAL: University of the Arts London](https://www.arts.ac.uk/partnerships/outreach/insights/how-to/challenges/challenges-creative-coding)_

### 2. In his paper, What is Generative Art: Complexity Theory as a Context for Art Theory(2003), Philip Galanter writes that " ... some maintain that this notion of structure is subjective and remains in the eye of the beholder. " Why might this be useful for the purposes of making generative art?\*\*

**Embed and refer to the three examples created above to support your explanation.**

- Structure being subjective to the eye of the beholder allows for more individuals to become more experimental when making generative art. Personally, structures would be defined as a recognizable shape or silhoutte in an artwork in which the audience are able to discern. With the high compressibility sketch, it is a canvas filled with structured tiles of simple squares that is much easier to decipher the scructure compared to the other two that lack a clear structure. The sketch for low compressibility and high effective complexity contains shapes that duplicate in random places which becomes more chaotic and messy.

**In your third example, what concepts and code are responsible for creating structure, in this sense?**

- For the third sketch, the concepts that were responsible for creating structure were the rect() and circle() functions. Within the function draw(), the code prompts the circles to be drawn at the mouse position with a diameter of 50, and the fill colour to red using the RGB values. The rectangles have similar attributes to the circles, instead they are coloured blue. These structures create a cohesive shape with how chaotic the p5.js sketch becomes once you drag your mouse around.

## Sabato Visconti

- The artist Sabato Visconti has specialised in various forms of media, including photography, illustration, 3D art, and most notably, glitch art. His ability to capture randomness whilst keeping some form of structure enabled him to achieve such complexity through his works. He has achieved this through several techniques such as pixel art, animation, neon colours, and photography to blend all these medias together.

![sabato-art](Pictures/sabato.png)

---

# Homework task 4b

### 1. Use techniques from Glitch, or Pixel , or both, to render a self-portrait on your blog.

<canvas id="glitch_self_portrait"></canvas>

<script type="module">

   const cnv = document.getElementById (`glitch_self_portrait`)
   cnv.width = cnv.parentNode.scrollWidth
   cnv.height = cnv.width * 9 / 16
   cnv.style.backgroundColor = `deeppink`

   const ctx = cnv.getContext (`2d`)

   let img_data

   const draw = i => ctx.drawImage (i, 0, 0, cnv.width, cnv.height)

   const img = new Image ()
   img.onload = () => {
      cnv.height = cnv.width * (img.height / img.width)
      draw (img)
      img_data = cnv.toDataURL ("image/jpeg")
      add_glitch ()
   }
   img.src = `/Pictures/joolieie.JPG` //my selfie

   const rand_int = max => Math.floor (Math.random () * max) 

// creates glitchy effect by taking random chunks of characters from base64 encoded image
   const glitchify = (data, chunk_max, repeats) => { 
      const chunk_size = rand_int (chunk_max / 4) * 4
      const i = rand_int (data.length - 24 - chunk_size) + 24
      const front = data.slice (0, i)
      const back = data.slice (i + chunk_size, data.length)
      const result = front + back
      return repeats == 0 ? result : glitchify (result, chunk_max, repeats - 1)
   }

//builds array of 12 pre-generated, randomly-glitched images
   const glitch_arr = []

   const add_glitch = () => {
      const i = new Image ()
      i.onload = () => {
         glitch_arr.push (i)
         if (glitch_arr.length < 12) add_glitch ()
         else draw_frame ()
      }
      i.src = glitchify (img_data, 96, 6)
   }
// boolean where false shows non-glitched image whereas true will show glitch
   let is_glitching = false
   let glitch_i = 0

   const draw_frame = () => {
      if (is_glitching) draw (glitch_arr[glitch_i])
      else draw (img)

      const prob = is_glitching ? 0.05 : 0.02
      if (Math.random () < prob) {
         glitch_i = rand_int (glitch_arr.length)
         is_glitching = !is_glitching
      }

      requestAnimationFrame (draw_frame)   
   }

</script>

### 2. How does rendering your likeness in this way affect its aesthetic register? In your discussion, please refer to:

**One or more readings from "Glitch Readings"**

- While reading Nick Briz's ['Thoughts on Glitch Art v2.0'](https://rmit.instructure.com/courses/151099/files/44700503?module_item_id=7237235), I found it interesting that he stated that glitches are not caused by computers, but rather by human error. This effect tends to make us think that the computer has made a "mistake" and setting the illusion that the user experience has unexpectedly been disrupted. This sentiment applies well to the self-portrait since the jarring effects of the glitches causes the audience to feel that they are watching the computer make errors, when in actuality, it was done intentionally through code.

**One or more readings from "Net Art Readings"**

- According to Cary Wolfe's ['Reflections on Art and Posthumanism'](https://rmit.instructure.com/courses/151099/files/44705319?module_item_id=7237540), they state that posthumanism is a "humanist fantasy of our ability to make transparent to master and make transparent to ourselves our deep, intractable cultural and philosophical inheritances." Basically, it means that we are utilising the admirable aspects of humanity to create art as a way to represent our current reality and humanity. I would say that the self-portrait is a post-digital piece that utilises technology and other post-humanistic aspects that truly embodies our current time.

**The concept of effective complexity**

- I think of the self-portrait as the structure (high compressibility) of the piece whilst the glitchy effects are the low compressibility elements that create the chaos within the piece. Through the blend of high and low compressibility elements, it creates an effective piece that reflects complexity.

**Ngai's three aesthetic registers**

- In terms of Ngai's three aesthetic registers, the chaotic nature of the self-portrait lies more into the zany aesthetic compared to the cute or interesting aesthetic. Ngai desribes the zany nature as manic and chaotic and is an aesthetic that is common in comedy. It creates a sense of chaos and overwhelming emotions when watching all these glitch effect unfold, especially in the self-portrait where all these glitches occur randomly which fits the zany aesthetic.
