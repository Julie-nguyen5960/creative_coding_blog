---
title: Week 3
published_at: 2025-03-26
snippet: Developing ideas!
disable_html_sanitization: true
allow_math: true
---
[Read Week 1](first-week)

[Read Week 2](second-week)
---
# Homework task 3a

**1. Describe how Rafael Rozendaal achieves a cute aesthetic register in artwork 'Passing':**

- visually

He uses a variety of bright colours that is complimentary to the other colours. When I look at this piece, I perceive those little squares as little people passing by or walking in a path which I think is adorable.

- sonically

There is no audio with this artwork.

- interactively

The simple mouse click to change the artwork's colors and square sizes is an interesting element that enhances the cute aesthetic register, shifting the perspective of how small and large these squares become.

![passing](Pictures/passing.png)

---

2. With regard to your AT1,explain how you plan on achieving the aesthetic register of cute:

**- visually**

In a visual sense, I plan to achieve the aesthetic register of cute through the use of rounded shapes and personifying my friend and I as small cute heads within a flower and star border. It will contain adorable elements such as a little drawing sticky note, pastel background and cute icons. The video displayed in the background is meant to replicate the animes we have watched together during quarantine.

**- sonically**

Sonically, I intend to utilise a sped up chatter sound effect similar to animal crossing once our icons are clicked on. The sound from the video in the background will be muted to emphasise more focus onto our icons and other interactive elements.

**- interactively**

In terms of interactivity, the interactive elements will comprise of mouse functions which involves mouseButton(), mouseClicked, mousePressed(), and mouseRealeased(). Most of these functions will account for the drawing pad in my canvas, whilst the 'mousePressed()' will be the only function applied to the cute icons. The user will be able to draw in the small notepad and click on the icons that will trigger a chatter sound.

3. Enlist some feedback on your ideas from a colleague. Ask them, for each of your examples above:

**- how well did you achieve a cute aesthetic?**
The person who was assigned to give feedback on my assignment 1 draft was Wonjun. He expressed that the flower and star border gives off a sentimental atmosphere. He also said utilising the animal crossing chatter matches the cute concept very well.

**- what could you try to increase the cuteness?**
Wonjun commented that I should set different chatter sounds for each charater just to bring out their individuality. Though I did not disclose previously in my blog, I did intend to use different sounds for each character.

**- how might you use implement these improvements using javascript?**
In order to implement these improvements, I would need to make new variables for each character to ensure that they can create a different sound. By using boolean logic, I can show different character icons, using the variables that I have declared.

---

## Homework 3b

---

**how your AT1 will use each of the following concepts:**

![code](Pictures/ss5.png)

**1. variables**

- Empty objects that represents values; holder of data or functions

My icons are classified as variables so they can carry out the function of triggering the sound file when being clicked on.

I'm planning for the notepad to become an object that users can draw on with the mouse, in order for that to happen, I need to set the notepad as a variable.

**2. functions**

- Assigning each variable to a function

So far, I have utilised the function draw(), function mousePressed(), function steup() and function preload(). Function draw is used for drawing up my image elements and certain animations that apply to the background and the change of icons. The function mousePressed() was used to prompt the mouse clicking on the icon and ensure that the icons switched once the mouse clicked.

**3. iteration**

- Repeating a block of code multiple times

Currently, my code does not use any iteration but I plan to implement this in the future to automate reptitive tasks and draw up the background elements like the taskbar and background picture. I will need to do this since my code is very reptitive.

**4. boolean logic**

- Boolean logic operators where variables only have values that are either either true or false.

I utilised the boolean logic in my code when I needed to assign my 'joolie' and 'nicole' icons variable to talk. I have also used '&&' to determine whether both operands are true, and the 'if' and 'else' conditions to ensure that the icons have switched states.

**5. arrays**

- consisting of a collection of elements, values and variables of the same type.

I have utilised array in my code through the use of const colours = ['#fffc8c', '#D8BFD8', '#FFB6C1', '#AEC6CF']; line. This was used so I can store the four colour values I wanted and apply it to the background colour.

**6. classes**

- Blueprint/ cookie cutter for creating objects with specific properties and behaviour.

Even though I have not used classes in my code, I plan to use it once I written all of my code and intend to factorise my code in a more efficient way. I will apply this to the 'joolie' and 'nicole' elements since they share similar attributes of switching between images and playing sounds.

![icons](Pictures/ss3.png)

**1. how well did you achieve cuteness in the visual, sonic, and interactive domains?**

Visually, I think I achieved the cuteness fairly well from using the lighter colours and rounded characters I have drawn. By using the animal crossing talking sound effect, I think it further pushes the cute aesthetic since animal crossing is a game known for its cute appearance. Although the interaction is simple where you click on the icons for the characters to start talking, I think it encapsulates cuteness perfectly just from the change of facial expression.

**2. what communities and learning resources did you draw on to do the bulk of your learning for this project?**

Majority of my resources comes from other P5.js sketches that I have found online in which I examined their code and what functions they used. I found ones that helped me learn how to upload images, [videos](https://editor.p5js.org/mai/sketches/SJJZiLLkz) and [sounds](https://editor.p5js.org/p5/sketches/Sound:_Load_and_Play_Sound). Another resource I relied on was CHATGPT that helped me with the mouse clicking function and debugging my code whenever I couldn't find the source to problem.

**3. what aspects have you enjoyed the most about this process? What have you found to be most surprising?**

The aspect I enjoyed the most was seeing the images I coded appear on the canvas and managing to get the mouse click function to work. It was satisifying to see the characters come to life and start talking. The most surprising aspect of this assignment was how observant you have to be when trying to detect any mistake in the code.

**4. what aspects have you struggled with the most? What have you found the most confusing?**

The things I have struggled the most was trying to find resources that would help me in coding more complicated functions. Debugging was also something I struggled with, even when the console.log would alert me where the issue lies. It is usually an issue that also lies elsewhere that affects that part of the code. Sometimes, I struggle to understand what some operands are doing to the code so it takes me longer to digest what is going on in the code.

<iframe id="at1draft" src="https://editor.p5js.org/Julie-nguyen5960/full/yXEZpTcyF"></iframe>

<script type="module">

    const iframe  = document.getElementById (`at1draft`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

## Assignment 1 reflection

Considering that this was my first time coding, I would say that this was a humbling experience and made me admire programmers much more for their ability to dissect code and create code out of nothing. It was difficult to learn all these different functions and operands within a short time span, but as I worked on this project more, I slowly gained a better understanding how to structure my code and this affected my P5.js sketch. I had the most fun when I started seeing my p5.js Sketch come to together from its cute visuals and the mouse interactions coming to life. I did need some help with different parts of code with the use of ChatGPT as it was difficult for me to trigger mouse interactions without any prior knowledge. Though I was happy to learn how to insert images and videos from other P5.js sketches I have found online.

Overall, I am pleased with how my P5.js sketch turned out especially with the many aspects such as the randomly generated pastel coloured background, the mouse interactions that allows you to draw on the canvas and tap on the characters. 

<iframe id="assignment1" src="https://editor.p5js.org/Julie-nguyen5960/full/63m6BTvxX"></iframe>

<script type="module">

    const iframe  = document.getElementById (`assignment1`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

[Assignment 1 full sketch](https://editor.p5js.org/Julie-nguyen5960/full/63m6BTvxX)

---
**What I learnt this week:**

1. Coding concepts

In class, we were taught the different coding concepts such as <mark>variables, functions, classes, iterations, boolean logic and arrays.</mark> Most of these functions were implemented in my code which helped me understand these concepts a bit better.

2. P5.js Sketch- trying to refine my code

I was trying to refine my code since I felt some aspects were reptitive or could be shortened, which made me compelled to use the classes function on the emojis in my sketch. I had to classify a class in a separate sketch file and link these files in the index.html file. Sometimes, I tend to forget that step. Though I was not confident in putting my other objects in a class, especially ones with different functions relevant to the interactive experience.

![class](Pictures/class.png)

