---
title: Week 2
published_at: 2025-03-07
snippet: Slowly easing my way into Coding!
disable_html_sanitization: true
allow_math: true
---

# Homework task 2a

**♦ cute visuals-**

To encapsulate cuteness, these visuals need to consist of mostly rounded lines and edges to make the object or character more approachable. The use of pastel colours will also aid in making the sketch appear more cute. Many cute mascots contain rounded features, big eyes and are usually short. Noteable characters that are considered cute, includes Pompompurin, ShinChan, Chiikawa and Mofusand. In my sketch, I plan to draw up a mascot with rounded features, with a face and drawn with soft lines. The concepts I will utilise for this sketch is Image(), loadImage(), random(), colorMode (HSB), and fill().

**♦ cute sounds-**

I think what makes a sound 'cute,' it is usually short, simple and quick. It also consists of a lighter sound, and is higher in pitch just like how Alvin and the Chipmunks covers and nightcore were popular back then. Most tiktok songs are sped-up songs whilst also adjusting the pitch to make the song sound more 'cute.' There are instances where Anime characters try to appear cute sounds through small breath sounds and unique eating sounds. In order to implement sounds into the sketch, I will need to use the functions of function setup(), loadSound() and let playing = false;.

 <iframe id="cute audio" src="https://editor.p5js.org/Julie-nguyen5960/full/i7ap2cpxO"></iframe>

<script type="module">

    const iframe  = document.getElementById (`cute audio`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 10 + 30

</script>

- raseldesigner93 (n.d) Cute Piano Illustration, Accessed 16 March 2025, [image one](https://www.vecteezy.com/vector-art/47882979-cute-piano-illustration-cartoons-clipart-and-line-art-design-for-microstock-adorable-piano-illustration-perfect-for-cartoons-clipart-and-line-art-designs)

- raseldesigner93 (n.d) Cute Piano Illustration, Accessed 16 March 2025, [image two](https://www.vecteezy.com/vector-art/47882979-cute-piano-illustration-cartoons-clipart-and-line-art-design-for-microstock-adorable-piano-illustration-perfect-for-cartoons-clipart-and-line-art-designs)

- [Piano Audio](https://www.youtube.com/watch?v=7w6rUfoQtxo)

- Code extracted from @arialabel's [sketch](https://editor.p5js.org/p5/sketches/Sound:_Load_and_Play_Sound)

**♦ cute interactions-**

In order to create cute interactions, the cute characters have to be interactive with the user like Bonzi buddy who is able to talk and dragged anywhere on the screen. I plan to have a similar mechanic of being able to drag the character around inside the canvas. I will utilise the mouseButton(), mouseClicked() and mouseDragged() to enable draggability and hopefully elicit some sound.

 <iframe id="cute" src="https://editor.p5js.org/Julie-nguyen5960/full/MzZSSwTjaC"></iframe>

<script type="module">

    const iframe  = document.getElementById (`cute`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 10 + 30

</script>

- [Gojo plush render](https://www.deviantart.com/marcopolo157/art/Gojo-Ball-Plush-Render-PNG-JJK-1047244907)

- (All these P5.js sketches are just there to let me have a grasp at the functions)

---

# Homework task 2b

Based on the description of a 'kindred spirit,' my mind gravitated toward my best friend who guided me on the path of self-discovery and served as a positive influence in my life. Our dynamic has changed alot over the past years; at first, I was the reserved, quiet friend whilst she was the outgoing and loud friend. Now, we are more open with each other since she has tuaght me to not be unashamed of who I am. It felt like a miracle to meet someone with so much in common, especially when we shared the same hobbies, interests, and sense of adventure. She was there when I had no one else to share my interest in anime with, encouraged me when I felt down, and gave me a positive outlook on life.

1.

**- what is the context of your kinship?**

I'm basing this assignment on a kinship shared between me and my friend, I see her as someone who has guided me through life and its circumstances. We remained close for more than a decade due to our shared effort of keeping each other in contact. Whenever we get the chance to hang out, it's always a pleasure to spend time with her. She also helped me further shape my identity through our exploration of different hobbies, ideas and many more.

**- what is your common purpose?**

We share the common purpose of wanting to live spontaneously and are willing to try the many things that life has to offer.

**- who or what is your shared challenge / adversary?**

Our shared adversity is mainly our self-esteem, tendency to hide our emotions and our need to constantly grow as a person. I believe that there's always room to improve as a person. We always try to uplift each other with positive affirmations and compliments, it always helps me gain more confidence in myself.

---

2.

![sitoncar](Pictures/sitoncar.jpg) _-When I sketched this out, I imagined the sky changing once you click the mouse onto the sky. However, I didn't gravitate towards this idea as it seemed less fun to make and required more drawing._

![herefm](Pictures/herefm.jpg) - _I really liked this idea due to how simple this idea is but can be executed in a cute fashion once I lay out the foundation for the code._

So if I was creating a sketch in tribute to my friend, I was planning to represent us either as an cute animal or as chibi communicating through a call. I also wanted to add a video player on the side to further establish what type of setting it is. I also want to utilise the random function to change the background colour to various pastel colours. I am trying to recreate this time in our life (2020), where we reguarly hopped onto a website called Here.fm to watch anime together. I think it will be a cute idea since Here.fm allowed for cute customisation choices in how you wanted to decorate the watch party room.

In addition to the sonic elements, I was hoping to add sounds that are quite similar to animal crossing's sped up speech when our icons are clicked. I'm not too sure about having audio play from the mp4 file, but most likely not just so the sounds aren't too distracting.

As for the mouse interactions, the plan is to make my friend's and my icons the interactive elements of this sketch. My aim is to ensure that the icons change once the mouse clicks on it and also allow users to watch the video in the background that is on loop to further immerse them in the chatroom.

 <iframe id="bunny test" src=" https://editor.p5js.org/Julie-nguyen5960/full/PFuiDUCQE"></iframe>

<script type="module">

    const iframe  = document.getElementById (`bunny test`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

_This is the general idea of what functions I would like to include in the final sketch where the video in the background loops, whilst you are able to interact with the icon that triggers a sound_

[link to full sketch](https://editor.p5js.org/Julie-nguyen5960/full/PFuiDUCQE) (Bunny video doesn't play in screenplayer)

3.

For the third part of this homework, we were assigned to analyse the code for the recreation sketch of '[Falling Falling](https://editor.p5js.org/Julie-nguyen5960/sketches/Xx6TxhhO1)' by Rafaël Rozendaal. I don't consider myself very skilled in coding so interpeting what certain codes will do was a challenge for me. Majority of my notes are guesses which I'm not most certain in, there were some line of codes I was more confident in knowing their functions and how it affected the sketch.

_Attempt at analysing code:_
![falling](Pictures/falling.png)

**List of lines of code I don't understand**

- faller.start_points = [

  { x: 0, y: height / 2 },
  { x: 0, y: 0 },
  { x: width / 4, y: 0 },
  { x: width / 2, y: 0 },
  { x: width \* 3 / 4, y: 0 },
  { x: width, y: 0 },
  { x: width, y: height / 2 },
  ]

- faller.end_points.push ({
  x: i \* width / 8,
  y: height
  })

- faller.curves = new Array (7).fill ().map (rand_curve)
  faller.phase = 0

- fallers.push (Object.assign ({}, faller))

- new_faller.curves = new Array (7).fill ().map (rand_curve)
  fallers.reverse ()
  fallers.push (new_faller)
  fallers.reverse ()

- fill (lerpColor (f.colours[0], f.colours[1], f.phase))
  beginShape ()
  vertex (0, height)
  f.start_points.forEach ((s, i) => {
  const p = find_point (s, f.end_points[i], f.phase \*\* f.curves[i])
  vertex (p.x, p.y)
  })
  vertex (width, height)
  endShape ()
  f.phase += 0.008
  if (f.phase > 1) redundant.push (i)

- redundant.forEach (n => fallers.splice (n, 1))

- function find_point (start, end, phase) {
  const delt = {
  x: end.x - start.x,
  y: end.y - start.y
  }
  const x = start.x + delt.x _ phase
  const y = start.y + delt.y _ phase
  return { x, y }
  }

- function rand_curve () {
  return random () \* 2 + 1
  }

---

**Resources that may help me understand these lines of code**

- CHATGPT
- W3School- Javascript Operations
- P5.js References
- P5.js Tutorials
- The Coding Train (YouTube)
