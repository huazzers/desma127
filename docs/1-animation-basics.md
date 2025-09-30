---
title: Key Principles of Interactive Animation
---

<script>hljs.highlightAll();</script>

<!--jump to anchor tag adjusted to header height offset-->
<script>
// Get the header element
let header = document.querySelector('header');

// Get the height of the header
document.querySelectorAll('a[href^="#"]')
.forEach(function (anchor) {
    anchor.addEventListener('click', 
    function (event) {
        event.preventDefault();

        // Get the target element that 
        // the anchor link points to
        let target = document.querySelector(
            this.getAttribute('href')
        );
        
        let headerHeight = header.offsetHeight*2;
        
        let targetPosition = target
            .getBoundingClientRect().top - headerHeight;

        window.scrollTo({
            top: targetPosition + window.scrollY,
            behavior: 'smooth'
        });
    });
});
</script>

# Key Principles of Interactive Animation

## Animation Fundamentals

### The 12 Principles

Developed by two Disney animators in 1981 who were studying the values outlined by *other* Disney animators from the 1930's onwards. 

![](./img/1-illusionoflife.jpg)

<br>

Given that these principles come from a very specific style of Disney animation, not all of these principles may be applicable to everyone. However, they are useful to consider as a general vocabulary for describing basic steps and thought processes behind animation practices.

<br>

#### 1. Squash and Stretch

The physical effects of pushing and pulling by gravity, velocity, and other forces acting upon a body. Describes the material and expressive quality of an animated object -- e.g. how elastic and heavy something is. 

![](./img/1_squashstretch1.jpg)

![](./img/1_squashstretch3.jpg)

![](./img/1_squashstretch2.jpg)

<br>

#### 2. Anticipation

Build-up momentum before release.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/0sCSK1Ox5Ts?si=dWlZx9jRKFY-DB-m" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<br>

#### 3. Staging

How are you setting up your scene to tell a story? What should your audience be looking at or paying attention to?

Think about how to communicate **key actions and story beats**, as well as **direct your audience's gaze** using cinematography, composition and framing, background set, as well as timing.

<figure>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/TJI_gygXsfs?si=f_J2-v9c-q2zy39b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<figcaption>Looney Tunes, Rabbit of Seville. "Be Vewy Quiet, I'm Hunting Wabbits!"</figcaption>
</figure>

<br>

#### 4. Straight ahead VS Pose-to-pose

**Straight ahead** is most common for effects animation -- start with one drawing and draw the next until you're done. It's a spontaneous, fluid, and almost unconscious way of animating, because there's no predefined keyframes to act as your blueprint. 

![](./img/smokeanimation.gif)

<br>

**Pose-to-pose** begins with the establishments of keyframes, followed by the filling in of empty gaps with in-betweens that. It's a very structured, calculated, and logical way of animating, giving clarity as to where our drawings will be at which time. 

![](./img/1_extremes.jpg)

![](./img/1_breakdowns.jpg)

<br>

These two approaches aren't mutually exclusive -- there are methods for blending both straight ahead AND pose-to-pose in the same animation.

Here's one example from pages 63 - 68 of the Animator's Survival Kit:

<figure>
    <img src="../img/1_posetoposedemo.jpg">
    <figcaption>Begin with Pose-to-pose to establish keyframes and timing of each step the character takes. This will become the reference guide for our straight ahead animation.</figcaption>
</figure>

<figure>
    <img src="../img/1_straightaheaddemo.jpg">
    <figcaption>...then, on top of these poses, animate each body part / action separately using the straight-ahead method to add secondary actions and fluidity to the motion.</figcaption>
</figure>

<br>

#### 5. Follow through and overlap

<blockquote><p>"An object in motion stays in motion"</p><figcaption>-- Isaac Newton (basically)</figcaption></blockquote>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/3GTkhSDBzYo?si=AVF2sc4TnhOlmeVy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<br>

When an action stops, the momentum of that action may propel other objects to continue moving.

![](./img/1_overlap.png)

<br>

#### 6. Ease in and ease out

<blockquote><p>"An object at rest will want to remain at rest, unless something causes them to move."</p><figcaption>-- Isaac Newton (basically)</figcaption></blockquote>

In general, actions should **start slowly, speed up, and then slow down again before stopping**. This gives the illusion of physical weight to our animated body. 

This is achieved by placing drawings closer together at the start and end of an action.

Remember our pendulum example from [Pose-to-pose](#4-straight-ahead-vs-pose-to-pose)? 

![](./img/1_easing.jpg)

![](./img/1_easing2.jpg)

<br>

#### 7. Arcs

Arcs look natural. Try to arc as many lines of action as possible.

![](./img/1_arcs.png)

<br>

#### 8. Secondary Action

Movement that is dependent upon some other, active movement. Consider the hierarchy within the animated body -- which body part should follow what? 

<figure>
<img src="https://64.media.tumblr.com/42d1da82d3739e574b486ec92cd2236c/tumblr_p7ag2ossXW1t1ig6no1_400.gifv">
<figcaption>-- Keke, <a href="https://k-eke.tumblr.com/post/172999953576/happy-tap-dancing-fox">Happy tap dancing fox</a>.
</figcaption>
</figure>

<br>

#### 9. Timing

<blockquote><p>"It's all in the timing and the spacing"</p><figcaption>-- Grim Natwick</figcaption></blockquote>

How many drawings will you choose to make between important poses, and where will you place them? How much **space** is there between animation frames **on the canvas, and on the timeline**?

Consider your **frame rate**, and whether you're animating on ones or twos.

* more in-between frames = smoother action
* less positional spacing in between frames on canvas = moves slower
* shorter duration in between frames on timeline = faster animation

![](./img/1_timing.png)

<br>

#### 10. Exaggeration

Pushing poses so they are as expressive as possible makes animation feel more alive.

![](./img/1_exaggeration.gif)

<br>

#### 11. Good (or "solid") drawing

A sense of **three-dimensionality**: form, volume, proportion, perspective. 

<figure>
<iframe title="vimeo-player" src="https://player.vimeo.com/video/36626926?h=c541297d32" width="500" height="360" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share"   allowfullscreen></iframe>
<figcaption>-- James Baxter, Spirit Roughs. Here's more of his pencil tests online: <a href="https://livlily.blogspot.com/2010/10/james-baxter.html">https://livlily.blogspot.com/2010/10/james-baxter.html</a></figcaption>
</figure>

<br>

**Character turnarounds**, for example, establish how a character should appear from different perspectives.

![](./img/1_turnaround.png)

<br>

**Clarity of pose**: line of action, silhouette.

![](https://www.animationmentor.com/wp-content/uploads/2017/07/Sebastian01.jpg)
<br>
![](https://www.animationmentor.com/wp-content/uploads/2017/07/Sebastian02.png)

<br>

**Avoid perfect symmetry** or "twinning", which makes drawings look flat; try twisting the body, or using Contrapposto (counterpose in English). 

<figure>
<img src="../img/1_twinning.jpg">
<figcaption>-- An example from "The Illusion of Life".</figcaption>
</figure>

<br>

![](https://www.animationmentor.com/wp-content/uploads/2017/07/DavidCatDrawing.jpg)

<br>

#### 12. Appeal

Appeal is subjective -- consider what makes a shape **memorable**. 

E.g. Interesting proportions, defined edges, simplified details, dynamic colors, etc.

![](./img/1_appeal.jpg)

<br>

---

### Quick review

Can you identify which principle(s) have been included in these videos?

- [Video 1](./img/triggerworkshop.mp4)
- [Video 2](https://www.youtube.com/watch?v=seA5BVFJSnQ)
- [Video 3](https://www.youtube.com/watch?v=csvOWBDx1oM)
- [Video 4](https://www.youtube.com/watch?v=V1RM_eIlYKw)

---

### Common Terminology in 2D Animation 

#### Frame

One drawing in a sequence on a timeline.

E.g. This bouncing ball animation is made up of 30 frames. 

![](./img/bouncingball.gif)<br>
![](./img/bouncingballframes.png)

<br>


#### Frame Rate

Defined in **frames per second (fps)**.

- **Ones**: a drawing every frame; <br>(e.g. in 24 fps, we'd have 24 drawings a second.)
- **Twos**: a drawing ever two frames. <br>(e.g. in 24 fps, we'd have 12 drawings a second, so it's technically 12 fps.)

<br>

#### Layer

A system managed by animation software that allows you to combine effects or drawings non-destructively.

Animations can be separated by body part, colour fill (e.g. base, shadow, highlights), etc.

<figure>
<img src="../img/1_animlayers.gif">
<figcaption>-- Mob Psycho 100 II Opening Music Video.</figcaption>
</figure>

<br>

<figure>
<img src="../img/1_animlayers1.png">
<figcaption>-- Taken from the <a href="https://www.live2d.com/en/cubism/about/">Live2D Cubism Editor website.</a></figcaption>
</figure>

<br>


#### Onion Skinning

An effect managed by animation software that allows you to see the frame before or after the current frame you are working on. This allows you to place your drawings more accurately.

![](./img/1_onionskin.png)

<br>

#### Keyframes

*("keys" for short)*

The main poses of your animation (or the "storytelling drawings" that show what's happening in the shot.)

In digital animation, these markers on a timeline indicate the beginning or end of an action.

![](./img/1_extremes.jpg)

<br>

#### In-between

*(verb = "tween")*

Frames that connect important poses (keyframes).

![](./img/1_inbetweens.jpg)

<br>

#### Interpolation

The approximation of unknown values between two known data points. 

In animation, the term "keyframe interpolation" is used to describe the distribution of in-between frames. 

Here's an example from [Eli Guerron](https://www.eliguerron.com/math-function-based-behaviors-for-ui-animations/):

<figure>
    <img src="https://images.squarespace-cdn.com/content/v1/5637a466e4b09f6317237330/1456660739445-HN6RYTXR6HN9AE3W701C/image-asset.gif?format=750w">
    <figcaption>-- Linear interpolation.</figcaption>
</figure>

<figure>
    <img src="https://images.squarespace-cdn.com/content/v1/5637a466e4b09f6317237330/1456660783485-49RR3MD08XGJU7MWX3JK/image-asset.gif?format=750w">
    <figcaption>-- Smoothstep interpolation.</figcaption>
</figure>

<br>

#### Smear

Frames that depict “blur” and use dramatic distortions or iteration to create the illusion of speed. 

Historically a budgetary necessity for limited animation to lower costs through fewer drawings, though some consider this a stylistic choice.

<figure>
<img src="../img/1_smear1.jpg">
<figcaption>-- Guy Buffet, Singapore Sling, among <a href="https://www.guybuffet.com/gallery/Limited-Edition-Prints/G0000gRfwWbFR9iw/">many other paintings of bartenders making drinks</a>.</figcaption>
</figure>

<br>

<figure>
<img src="https://www.traditionalanimation.com/wp-content/uploads/2017/08/TheCatsTale1941WanerBros-768x191.jpg">
<figcaption>-- Dry brush effect</figcaption>
</figure>

<br>


<figure>
<img src="https://www.traditionalanimation.com/wp-content/uploads/2017/08/SmeareBugs.jpg">
<figcaption>-- Animation smears</figcaption>
</figure>

<br>


<figure>
<img src="https://www.traditionalanimation.com/wp-content/uploads/2017/08/MultiplesRoadrunner.gif">
<figcaption>-- Multiples</figcaption>
</figure>

<br>

<figure>
<img src="https://www.traditionalanimation.com/wp-content/uploads/2017/08/DryBrushchuckjones.gif">
<figcaption>-- A combination of dry brush, smears, and multiples</figcaption>
</figure>

<br>

#### Morph

Visual effects technique which transforms one shape into another in a smooth transition.

![](./img/1_morph.webp)

<br>

![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmedia.tenor.com%2Fjx-H08vi0E4AAAAC%2Fbaby-spirited-away.gif&f=1&nofb=1&ipt=523266a842b5859bb07213480a2c04bf9362fc17fd96463fd689ba5a64442fee)

<br>

#### Boil

A stylistic decision to trace over lines or repeat textures repeatedly, to add motion to an otherwise still frame.

<img src="../img/1_boil.gif" width="300">

<br>

#### Loop

The first and last frame of an animation are sequential, allowing the animation to repeat seamlessly and endlessly.

<figure>
<img src="../img/1_annafirth1.gif" width="400">
<img src="../img/1_annafirth2.gif" width="400">
<figcaption>-- Anna Firth
</figcaption>
</figure>

<br>

<iframe title="vimeo-player" src="https://player.vimeo.com/video/296503067?h=75ae0f4feb" width="640" height="360" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share"   allowfullscreen></iframe>

<br>

Many animated films use loops to create repetitive movements (or add line boil animations to an otherwise still moment.)

Can you identify moments where animation loops have been used in these films? 

<iframe title="vimeo-player" src="https://player.vimeo.com/video/304241937?h=01d932e35e" width="640" height="360" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share"   allowfullscreen></iframe>

<br>

<iframe title="vimeo-player" src="https://player.vimeo.com/video/74627307?h=cbe69a44ac" width="640" height="360" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share"   allowfullscreen></iframe>

<br>

<iframe title="vimeo-player" src="https://player.vimeo.com/video/81986358?h=8b5ead0cb0" width="640" height="360" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share"   allowfullscreen></iframe>

<br>

So, how does looping animation work in games and interactive projects?

<br>

---

## How Interactive Animation Works

In interactive projects, animations are used as **assets** (ie. resource material) that can be programmed and manipulated through the development software. 

These animation assets are typically designed to be used as components for a type of computation model called **finite state machines**: 

- they have a **finite list of possible states**. 
- they can only be in **ONE state** at any given time. 
- they can **transition** from one state to another in response to some **inputs**. 

![](https://huazzers.github.io/desma126/img/state-flowchart.png)

<br>


When we get into Unity, you'll arrange your animations into this finite state machine called the Animator component. 

![](./img/1_unityanimator.jpeg)

<br>

The animator can transition from one state to another either at the end of an animation, or using conditional parameters such as: 

- **Bools**: a value that can either be true (1) or false (0).
- **Triggers**: fires once, then automatically turns off immediately after. 

*More on these next week...*

<br>

Generally, we can organize animations for interactive projects into two different state categories -- **Idle states**, and **Active states**.

### Idle State

When an interactable asset is **at rest** or **not receiving any player input**, we call this an Idle animation, Idle state, or just "an idle." 

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/MB5Okiv7TpU?si=1WmqilT1T2YuEkrz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<br>

Technically, an object that is "idling" doesn't need to animate at all -- but it can! 

It's common to see characters in video games idle, but really, *any* animation can loop, so *anything* can idle.

### Active State

An interactable asset that responds to a certain input is said to have transitioned from an "idle" to "active" state. 

![](./img/1_idleactivestate.gif)

<br>

---