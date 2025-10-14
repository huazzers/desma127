---
title: Worldbuilding through Player Involvement
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

# Worldbuilding Through Player Involvement

## Player Involvement

<figure>
<img src="../img/playerinvolvementmodel.jpg" width="800px">
<figcaption>-- Gordon Calleja's Player Involvement Model, taken from his book "In-Game: From Immersion to Incorporation".</figcaption>
</figure>

<br>



<figure>
<img src="https://indiedevstories.com/wp-content/uploads/2011/03/flow-channel1.png" width="800px">
<figcaption>-- The flow channel, from Jesse Schell's book "The Art of Game Design." Based on Mihaly Csikzentmihalyi's concept of "flow"</figcaption>
</figure>

<br>



<br>


<figure>
<img src="https://unit9.com/wp-content/uploads/waytogo4.jpg" width="800px">
<figcaption>-- Way To Go.</figcaption>
</figure>

---

## A brief history of 2D navigation and collider-based events in games

<figure>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/cWOkHQXw0JQ?si=ykfloVfYlzxnBCmm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<figcaption>-- Nintendo, Super Mario games.</figcaption>
</figure>

<br>

<figure>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/U7gAoTWFTwY?si=_W3MzBW-53im_2EU&amp;start=324" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<figcaption>-- Infinite Fall, Night in the Woods.</figcaption>
</figure>

<br>

<figure>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vUgTjnim3lw?si=su_PEUgu9FO269cC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<figcaption>-- Toby Fox, Undertale</figcaption>
</figure>

<br>


A question for all of you to think about--

How can we make use of player agency, avatar performance, and scene design to tell a story related to **space, control, and collecting**?

<br>


## Past Student Projects

for inspiration...!

<figure>
<iframe src="https://player.vimeo.com/video/933880233?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="560" height="421" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" title="As Above As Below by Katie Kang"></iframe>
<figcaption>-- Katie Kang, As Above As Below.</figcaption>
</figure>

> ***As Above As Below** explores the modern Western idea of the human body and its relation to cleanliness, holiness, and purity as well as its relationship to filth, waste, and “impurities.”*

<br>

<figure>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/6TIi37UYCGo?si=KIN7WwMFg7YiVKU0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<figcaption>-- Michael Luo, <a href="https://cathoderadiator.itch.io/days-dark">Days Dark.</a></figcaption>
</figure>

> ***Days Dark** is a short, alternative walking simulator game set in a mysteriously barren land. The protagonist (player) is a middle-aged woman carrying a basket of valuable food to feed her family. She needs to survive this treacherous land filled with hungry dogs, hungry ghouls, and an oppressive king demanding her tribute. The gameplay is designed to imitate walking and invoke the physical pain of running when encountering enemies by rapidly altering two buttons to move forward.*
> 
> *Days Dark is an ode to the forgotten matriarchs, who carried generations of family, including my own, through the darkest days. Loosely based on the events during the Great Leap Forward in my home province, this game explores the pain, oppression, and marginality experienced by my grandmother, her sisters, and their mother’s forgotten sacrifices living under traditional patriarchy.*

<br>

<figure>
<iframe src="https://player.vimeo.com/video/541877782?h=c2e5c51072&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="560" height="348" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Panopticon"></iframe>
<figcaption>-- Ainsleigh Douglas, Panopticon.</figcaption>
</figure>

> ***Panopticon** is a 2D illustrated, 3rd person adventure game with interactive elements that are revealed as the space is navigated. Play as a bot traveling through an alternate reality internet simulation. The world you defined as home, made up of 0’s and 1’s, has become physical reality. Your goal is to make it through the seven levels of the deep web without being noticed by the guard tower in the center. Do your best to travel through this panopticon-like maze on your path to self discovery of what it means to be a mechanism of the internet.*

<br>

<figure>
<iframe src="https://player.vimeo.com/video/662741617?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="560" height="287" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Grandma&#039;s Ocean by Yuchi Ma"></iframe>
<figcaption>
-- Yuchi Ma, Grandma's Ocean.
</figcaption>
</figure>

> ***Grandma’s Ocean** is an attempt at seeking connections and re-imagining with personal narrative through the medium of game-making, collage and personal narrative. 3 women in 3 different time periods, the game characters’ lives and paths mirror and build on top of each other. Their generation connection cycles through different political and historical influences, carrying love, trauma, and tattered ideas of home to each of their lives and individual actions. This is my attempt to close some gaps between myself and her and her.*