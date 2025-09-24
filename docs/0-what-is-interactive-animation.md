---
title: What Is Interactive Animation?
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

# What Is Interactive Animation?

---

## What is Animation?

> "Animation is a filmmaking technique whereby still images are manipulated to create moving images."
> 
> -- Wikipedia, "[Animation](https://en.wikipedia.org/wiki/Animation)"

![](./img/bouncingball.gif)

![](./img/bouncingballframes.png)

<br>

<figure>
    <img src="../img/animators-survival-kit.jpg">
    <figcaption>-- Richard Williams, "The Animator's Survival Kit", p. 9.</figcaption>
</figure>

<br>



<figure>
    <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/aEAObel8yIE?si=TFnF5_vc94H2LF_b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    <figcaption>-- Emile Cohl, "Fantasmagorie" (1908)</figcaption>
</figure>

<figure>
    <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/32pzHWUTcPc?si=shXPzw20Rcrvi6pv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    <figcaption>-- Windsor McCay, "Gertie the Dinosaur" (1914).</figcaption>
</figure>


