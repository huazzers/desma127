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

# Project 2: 3D Interactive Animation

<div class="duedate">
<p>📌 <b>SKETCH/PROPOSAL DUE:</b> Week 6 Thursday, November 6</p>
<p>📌 <b>FINAL PROJECT BUILD + DOCUMENTATION DUE:</b> Week 10 Tuesday, December 2 </p>
<p>Submit Final Submission Here (TBD)</p>
<blockquote>Please read the <a href="../how-to-submit">How To Submit</a> page for more detailed instructions.</blockquote>
</div>

## Prompt

Our second project focuses on **3D animation workflows** in Unity -- at minimum, two CG objects that function as the central focus of an interactive animated project. 

You are encouraged to implement an experimental controller, but it is not required. 

You're welcome to work in pairs or teams for larger-scope projects, please consult the TA / instructor for further guidance.

There is no prompt for this project, but I want you to consider two things from the concept to execution phase of your project:

- **Presentation**: Where will your project be seen and who will see it?
- **Interfacing and Control**: What does your audience get from interfacing with your work that they wouldn’t get from a non-interactive animation? How do the physical interactions through the controller relate to what your player experiences through the digital screen? 

<br>

**Inspirations:**

- [Danielle Brathwaite-Shirley](https://www.daniellebrathwaiteshirley.com/blacktransarchive-com)
- [*Hard Lads*](https://radiatoryang.itch.io/hardlads) by Robert Yang
- [Akihiko Taniguchi](https://vimeo.com/430233014?fl=pl&fe=sh)
- [Carl Burton](https://www.carlburton.io/islands-nonplaces-1)
- [*Groom*](https://games.ucla.edu/game/groom) by Miles Peyton
- [David O'Reilly](https://davidoreilly.itch.io/mountain)

<br>

## Requirements

**Your interactive animation is required to:**

- include **at least two CG objects you created**, each with **at least two animation states.**
- use a **button press, mouse click, or other input device to activate/animate/navigate your CG object**
- consider the **"start" and "end goal"** of your project. Does it end? 

<br>

**Requirements to score an A:**

- have sound;
- have a concept, story, or meaningful origin behind your decisions;
- implement 3D animation techniques.

<br>

**Your project is NOT required to:** 

- *only* use 3D animation techniques -- you're welcome to combine 2.5D aesthetics or prior 2D workflows as long as the requirements above have already been met. 

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