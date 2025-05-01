---
title: Week 7
published_at: 2025-04-21
snippet: Sound
disable_html_sanitization: true
allow_math: true
---

# Homework 7a

### **1. how will you make the sound design for your AT2 function in a chaotic aesthetic register? What does it mean to be chaotic in the sonic domain? In your discussion, please make reference to:**

- As of currently, I am unsure how I will create such sound that will evoke chaos as I do not have a clear idea on what my sketch will look like.

**Structure - what structures our perception of sound?**

- Amongst many people, our perspection of sound can vary depending on different cultures, environment, emotions and the delivery of the sound.

**Noise - what differentiates noise from sound, or music?**

- What truly differentiates a noise from a sound is based on context, but usually a 'noise' is associated with an unpleasant or disruptive sound. On the other hand, sound is defined as anything that is audible and music comprises of instrumental sounds that is organised is a systematic way.

**Voice - what makes voice a separate category of sound?**

- The voice would be a separate catergory of sound because of how a voice is delivered, through the human body. This medium carries the language, emotion and is a source of communication.

### **three examples, which can (but don't have to) be taken from the following list:**

**MyNoise Generators: Water**

- This generator has buttons that you can adjust to increase certain sounds' decibels such as footsteps, waterfall, creek and many more. These elements add a more scenic value to these sounds compared to the other two where they intentionally distort these sounds.

![water](Pictures/water.png)

**Pink Trombone**

- This mode of distorting sounds simulating the anatomy of the human mouth. It allows the user to manipulate the movement of the tongue and the oral cavity, it also provides the option to adjust the pitch of the voice which I found really cool.

![pink-trombone](Pictures/pinktrombone.png)

**How to Kill a Zombie**

- To further push the glitchy effects, the audio is tampered with by applying various effects such as reversing it, 2x speed, rewinding, loud noises (beeps) and much more.

![zombie](Pictures/zombie.png)

**2. implement an interactive sound design experiment in your blog.**

- you will need to get some form of user gesture for Web Audio API to run.

<h2>Play a Sound with Tone.js</h2>
<button onclick="playNote()">Press me (C4)</button>

<script src="https://unpkg.com/tone"></script>

<script>
	function playNote() {
		const synth = new Tone.Synth().toDestination();
		synth.triggerAttackRelease("C4", "8n");
	}
</script>

- you can use a library, such as Tone.js or Pizzicato.js, or you can use Web Audio API, or you can use AudioWorklet.

- use a sinusoid to push your sound design into chaos and back every 24 seconds.

- explain your code with the help of syntax-highlighted, commented code blocks

- evaluate the success of your experiment with reference to your discussion in task 1

---

# Update on assignment 2

**25/4/2025**

I had trouble on importing RiTa onto my script.js file and tried many methods from the RiTa github, but to no avail. It would not let me use normal p5 functions so I felt lost when trying to find other solutions, especially when asking CHATGPT. I finally asked Tom to help me with setting up RiTa since I wanted to use it for my assignment as I felt it best suited the 'Information and Thinking' prompt. Turns out I was importing RiTa the wrong way and was not using ESM, plus I was also forgot to import p5 onto the file as well (gojo.txt is a tester). ESM uses p5 in a slightly different way so that is something I have to adapt to.

![mistakes](Pictures/mistakes.png)

Now I feel that I can get started on my assignment properly. I was now able to import my .txt file into the code that will now show up in the canvas. I feel more confident in carrying out my vision for the assignment. For my assignment, I am going to try encapsulate how information is constantly being passed over but the truth can be manipulated or morph into something completely different, thus an information overload for the reciever. I will do this by making the text itself look glitchy and bounce off the canvas. On top of that, I will probably add some other glitch effects onto the canvas itself to further push the chaos and making the text slightly indiscernable. I had to get CHATGPT to generate the code for the bouncing animation since I did not know how to do it.

![code](Pictures/code.png)

For example, [Frisk-256's](https://editor.p5js.org/Frisk-256/sketches) sketch has an aspect I like where the code manipulates the pixels hence, creating a glitchy animation. I may implement something like this in my net art.

<iframe id="glitch" src="https://editor.p5js.org/Frisk-256/full/vS6fV5h0E"></iframe>

<script type="module">

    const iframe  = document.getElementById (`glitch`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

---

# Homework 7b

### In her essay on Sianne Ngai: Zany, Cute, Interesting, McKenzie Wark writes: "Unlike the interesting, the zany really works against its constraints."

**1. What do you think she means by this?**

Based on this statement, I think that it means that the concept of 'interesting' works within its limits whereas, zany is chaotic, unpredictable and pushes through its limits. 

**2. In what ways would you consider the chaotic and the zany to be similar? In what ways are they different?**

They both aim to be disorderly, excessive and unpredictable in which pushes the boundaries; making the audience feel overstimulated and overwhelmed. However, I think the connotations along with these words could be the differing factor; chaotic implies stressful and a disorienting feeling whilst zany sounds more playful and fun.

**3. In what ways would you consider your AT2 to be zany?**

I think the appearance of buffering colours on the words could be considered zany and its shaky animation. The words bouncing around the canvas could also be described as playful and fun. 


**4. What might be some ways to make your AT2 more zany?**

I think applying more colours to the canvas could possibly heighten the zany aesthetic register, but I am not too sure if it will work out since I don't want it to become too chaotic or epileptic .

### Please write an accompaniment to your AT2. Include examples of how and where it uses:

**- variables**

![variable](Pictures/variables.png)

I tend to declare my variables on top of my code so it looks more organised. These variables consist of Serres' texts, synth, words, wordObjects, pixels and the animation. Once again, this is used so that I can apply different attributes to certain objects.

**- iteration**

![for loop](Pictures/for-loop.png)

I have applied the for loop multiple times for this net art, one occurs at line 34 in which is to ensure that it is repeating every word, creates an object for each word and controls its movement. Another use of the for loop occurs at line 81 and 89. 

**- functions**

![functions](Pictures/function.png)

This code utilises functions such as function drawWords(), function capturePixels() and function glitchSlices(). Most of these functions were used to draw up the words and animate the pixels and glitches. 

**- boolean logic**

![variable](Pictures/variables.png)

The one time I used boolean logic is within the variables for "let animate= false." By setting it as false, I am setting the initial state to false where it isn't animated unless the mouse is pressed.

**- arrays**

This code does include some arrays such as let serresText = []; let words = []; let wordObjects = []; and let prxl = []; These variables hold multiple elements.

**- classes**

No classes were used to create this net art.

**- recursion**

Recursions is a function that calls itself to solve a problem in smaller steps.

No recursions were used to create this net art. 


**How it responds to the chosen text**

I have chosen to use the p5 library RiTa and glitches to convey how I agree with Serre's sentiment on how information is chaotic through multiple means. By making the actual words glitchy and incoherent, it conveys to the viewers how information becomes messy and indecipherable. 

**Why you consider it to be post-digital**

I would consider any artwork that utilises different forms of coding languages or technology to be post-digital, it has become normalised to use digital sources to create art. In a way, it shows how far humanity has come in terms of technological advancement.