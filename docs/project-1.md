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

# Project 1: WarioWare

<div class="duedate">
<p>📌 <b>SKETCH/PROPOSAL DUE:</b> Week 2 Tuesday, October 7</p>
<p>📌 <b>FINAL PROJECT BUILD + DOCUMENTATION DUE:</b> Week 4 Tuesday, October 21</p>
<p>Submit Final Submission Here (TBD)</p>
<blockquote>Please read the <a href="../how-to-submit">How To Submit</a> page for more detailed instructions.</blockquote>
</div>

## Prompt

<figure>
<div class="div-container">
    <div style="width: 47.5%">
        <img src="../img/warioware_grab_win.gif" style="height: 250px;">
    </div>
    <div style="width: 47.5%">
        <img src="../img/warioware_grab_lose.gif" style="height: 250px;">
    </div>
</div>
<figcaption>-- Two different end scenes from the same minigame in <a href="https://www.youtube.com/watch?v=s75wwkug4r4">WarioWare, Inc: Mega Microgames!</a> (2003). If the player successfully presses the grab button in the correct timeframe, Wario smiles smugly; if the player misses, Wario sweats embarrassedly.</figcaption>
</figure>

In reference to the original video game series released by Nintendo, WarioWare describes a genre of videogames that feature a compilation of shorter minigames played in quick succession. Each minigame is speedy and simple -- only requiring one or two actions to complete within a seconds-long countdown timer. 

For our first project, each of you will create **a short 2D interactive animation** for a warioware-style project. 

Rather than adapting existing warioware scenes, the intention of this project should be to **experiment and explore your own angles of interest (formal and/or conceptual) within the limitations of this framework**. While observing the [project requirements](#requirements) below, find something meaningful, interesting, or personal to express with animation.

<br>

**Inspirations:**

Consider the creative decisions made in the following examples that communicate their respective rules and intentions for player interaction:

- How do the **pacing and aesthetic design** set the overall tone of the project? 
- What are the **cues (audio, visual, social, etc.)** that suggest how players should act in this space? 
- How much **agency** are players allowed to behave and express themselves differently? How does that transform or shape meaning in this project?

<br>

<figure>
    <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2F64.media.tumblr.com%2F0678b7aed62661df70fce02d0c19d41e%2F1bafdeedc401cedf-53%2Fs500x750%2F54c1a9228ed0e5cef6701643752d8eda899dd26c.gifv&f=1&nofb=1&ipt=79fd89982be30e05df1effbc0f9168b3b9e238b3d9987973972833a6aaf4ecde">
    <figcaption><i><a href="https://papercookies.itch.io/spookware-watch-party">SPOOKWARE</a></i> by BEESWAX GAMES. 
    </figcaption> 
</figure>

<br>

<figure>
    <img src="../img/cooking-mama.gif">
    <figcaption><i>Cooking Mama</i> for Nintendo DS.
    </figcaption> 
</figure>

<br>

<figure>
    <img src="../img/10mississippi.gif">
    <figcaption><i><a href="https://knarniapop.itch.io/10-mississippi">10 MISSISSIPPI</a></i> by Karina Popp. 
    </figcaption> 
</figure>

<br>

<figure>
    <img src="../img/noonecanstopmrdomino.gif">
    <figcaption><i><a href="https://www.youtube-nocookie.com/embed/7ff3UQUPdio?si=ywDCgUWrwZFdhAIa&amp;start=1007">NO ONE CAN STOP MR. DOMINO!<a></i> (1998) by Artdink.
    </figcaption>
</figure>

<br>

<figure>
    <img src="../img/kuukiyomi.gif">
    <figcaption><i><a href="https://store.steampowered.com/app/1384380/KUUKIYOMI_2_Consider_It_More__New_Era/">KUUKIYOMI 2: Consider It More!</a></i> by G-MODE. GIF is captured from <a href="https://www.youtube.com/watch?v=fm6bvRulO40">this playthrough video</a> by Retort on YouTube. 
    </figcaption> 
</figure>

<br>

<figure>
    <img src="../img/Plug-and-Play.gif">
    <figcaption><i><a href="https://plugplay.ch/">PLUG & PLAY</a></i> by Mario von Rickenbach and Michael Frei, based on the latter's <a href="https://vimeo.com/118453180?fl=pl&fe=sh">identically titled film</a>. 
    </figcaption> 
</figure>

<br>

<br>

## Requirements

**Your interactive animation is required to:**

1. have a **"start scene"**;

    > Keep any textual instructions within **1~3 words**!

2. have a **timed event**, ie. the duration in which a desired action must be completed in order to "win", otherwise the player "loses";

    > While 8~12 seconds is standard for warioware minigames, for this project, you're welcome to extend that timeframe **up to 2 minutes**. 

3. have an **"end scene"** be activated at the end of the timed event;

4. implement **ONE (1)** of the following formats:

    <blockquote>
    <div class="assign">**A. Point-and-click Mouse Interaction**</div><br>Design a 2D environment that reveals a secret or a story when explored with a mouse. Clicking objects will reveal details or surprises.

    **OR**

    <div class="assign">**B. WASD + Arrow Key Navigation**</div><br>Move a 2D object around an environment with arrow keys / WASD on your keyboard. Collisions in the environment trigger events, such as a new asset appearing or a new scene starting. 
    </blockquote>

<br>

**Requirements to score an A:**

- have **sound**;
- have a **concept, story, or meaningful origin** behind your decisions;
- contain **at least TWO (2)** assets that have active and idle states;
- implement **2D animation techniques**.

<br>

**Your project is NOT required to:** 

- have a series of "minigame" scenes, nor have a comedic tone and speedy pace like a classic warioware minigame;
- use explicit videogame-y language like "WIN", "LOSE", "SCORE", or visible countdown timer UI -- consider the premise of your project, then choose your words and images wisely... or get really experimental with it!
- implement both point-and-click mouse interaction **AND** WASD + arrow key navigation... but you can if you want to!


<br>

**Tips:**

- Use **score keepers or collision / trigger collider events** to activate your ending scenes. 
- Consider having **different ending scenes for different outcomes**, eg. whether the player successfully completes the minigame within the time limit.
- **Start from the scripts that will be shared in our tutorials**, and then make any necessary edits from there later on. 
- **Consider your audience and how it should be interacted with.** What do you want them to feel/know/discover? How can you design your project and interactions to communicate your story, feelings, or even a joke? 

<br>

## Deliverables

#### Sketch/Proposal

Bring to class for one-on-one check-in: 

- any **sketches, assets, prototypes, and works-in-progress** to illustrate your project's direction; 
- a **tentative project timeline** that breaks down your anticipated project workload into a schedule of smaller checkpoints leading up to the final project deadline, ie. what you aim to get done by when.

#### Final Project Build + Documentation

Refer to [How to Submit](how-to-submit.md) for the submission checklist, and instructions for exporting your files correctly.

<br>

## Evaluation

Your final project will be evaluated according to the guidelines listed in the [course syllabus](./syllabus.md/#evaluation-criteria).

---