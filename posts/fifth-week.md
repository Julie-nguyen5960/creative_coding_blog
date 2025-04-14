---
title: Week 5
published_at: 2025-04-10
snippet: more coding
disable_html_sanitization: true
allow_math: true
---

<!-- <script src="./p5.js"></script>

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
</script> -->

---

# Homework 5a

**1. Choose a specific work from a post-digital artist and describe it, referring to Florian Cramer's essay What is Post-Digital? to justify why you think this artist classifies as post-digital.**

## Matt Kane (@mattkaneartist)

![matt kane art](Pictures/matt.png)

**"Gazers"**- An artful interpretation of the moon phases that utilises cool colours and implements a hazy glitch effect, in which overlays the moon encased in a lattice box.

- According to Florian Cramer's 'What is post-digital' essay, she defines it as the "messy state of media, arts and design after their digitisation" and I believe that Matt Kane is a perfect example as a post-digital artist. This artist produces all his generative artworks digitally, using p5.js to create the glitch effect. I've noticed that the artist tends to put the hashtag of #cryptoart or #nftart which reflects a shift transcending the analog era of art.

**2. what technology are they using to produce their work?**

- P5.js
- Javascript

**Hypothetically, if they were using javascript, what APIs & libraries could they use?**

- Web Animations API
- WebGL
- P5js
- PixiJS

**3. use RiTa.js. to generate a post-digital poem responding to the work in your blog.**

<script type="module">
  import { RiTa } from "https://esm.sh/rita";
  console.log (RiTa)

const template = "The [adjective] [noun] [verb] [adverb].";

function generateSentence(): string {
  return template
    .replace("[adjective]", RiTa.randomWord({ pos: "jj" }))
    .replace("[noun]", RiTa.randomWord({ pos: "nn" }))
    .replace("[verb]", RiTa.randomWord({ pos: "vbz" }))
    .replace("[adverb]", RiTa.randomWord({ pos: "rb" }));
}

console.log(generateSentence());

</script>

---

# Homework 5b

**1. pick a three.js, and implement it directly in your blog.**

- ['Littlest tokyo'](https://sketchfab.com/3d-models/littlest-tokyo-94b24a60dc1b48248de50bf087c0f042) by Glenatron

<!-- <script type="module">

			import * as THREE from 'three';

			import Stats from 'three/addons/libs/stats.module.js';

			import { OrbitControls } from 'three/addons/controls/OrbitControls.js';
			import { RoomEnvironment } from 'three/addons/environments/RoomEnvironment.js';

			import { GLTFLoader } from 'three/addons/loaders/GLTFLoader.js';
			import { DRACOLoader } from 'three/addons/loaders/DRACOLoader.js';

			let mixer;

			const clock = new THREE.Clock();
			const container = document.getElementById( 'container' );

			const stats = new Stats();
			container.appendChild( stats.dom );

			const renderer = new THREE.WebGLRenderer( { antialias: true } );
			renderer.setPixelRatio( window.devicePixelRatio );
			renderer.setSize( window.innerWidth, window.innerHeight );
			container.appendChild( renderer.domElement );

			const pmremGenerator = new THREE.PMREMGenerator( renderer );

			const scene = new THREE.Scene();
			scene.background = new THREE.Color( 0xbfe3dd );
			scene.environment = pmremGenerator.fromScene( new RoomEnvironment(), 0.04 ).texture;

			const camera = new THREE.PerspectiveCamera( 40, window.innerWidth / window.innerHeight, 1, 100 );
			camera.position.set( 5, 2, 8 );

			const controls = new OrbitControls( camera, renderer.domElement );
			controls.target.set( 0, 0.5, 0 );
			controls.update();
			controls.enablePan = false;
			controls.enableDamping = true;

			const dracoLoader = new DRACOLoader();
			dracoLoader.setDecoderPath( 'jsm/libs/draco/gltf/' );

			const loader = new GLTFLoader();
			loader.setDRACOLoader( dracoLoader );
			loader.load( 'models/gltf/LittlestTokyo.glb', function ( gltf ) {

				const model = gltf.scene;
				model.position.set( 1, 1, 0 );
				model.scale.set( 0.01, 0.01, 0.01 );
				scene.add( model );

				mixer = new THREE.AnimationMixer( model );
				mixer.clipAction( gltf.animations[ 0 ] ).play();

				renderer.setAnimationLoop( animate );

			}, undefined, function ( e ) {

				console.error( e );

			} );


			window.onresize = function () {

				camera.aspect = window.innerWidth / window.innerHeight;
				camera.updateProjectionMatrix();

				renderer.setSize( window.innerWidth, window.innerHeight );

			};


			function animate() {

				const delta = clock.getDelta();

				mixer.update( delta );

				controls.update();

				stats.update();

				renderer.render( scene, camera );

			}


		</script> -->

**2. consider the piece of glitch art below by Sabato Visconti**

![flower](Pictures/flower.gif)

**What does having the 3D form glitch out like this do in terms of aesthetic register, and effective complexity?**

- For the aesthetic register, this would appeal more to zany and the interesting aesthetic due to its chaotic yet complex nature. Whilst this glitch art is chaotic with its glitchy effects, it also transforms into interesting shapes that keeps engagement up.

- As for effective complexity, it works well in establishing structure which is the black rose, but it quickly transforms into unrecognisable shapes or reduces its polygons from the 3D model.

**How do you think it works, under the hood?**

- I think the animations was achieved using WebGL since it allows for 3D model renders and is able to run on the web browser.

- I'm guessing they had to preload the 3D model into the code, create code for it to rotate and ensure that glitches/distortions occur at certain intervals.

- Create new images for each phases of distortions??

- Not sure specifically what code they would use to rotate.
