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

# Reading / Media Response

## Reading / Media 1

<!--
<div class="duedate">
<p>📌 <b>DUE:</b> Week 2 Tuesday, October 7</p>
<p><a href="https://docs.google.com/forms/d/e/1FAIpQLSf-aQnjMvUGLt_pN5MVnybPk62gFD3cdg7uOem0RNcTDoZitw/viewform?usp=sharing&ouid=111038396537777799192">Submit Final Submission Here</a></p>
</div>

Reading / Media 1 comes in TWO parts: 

1. a solo reading response; and
2. a group media response.

### PART 1: SOLO READING RESPONSE

Read **at least one** of these short essays about ideation/building ideas by these animators published in **Mostly Moving**, an independent animation journal:

- Caleb Wood: [Looking at Shit: Conception of Ideas](https://mostlymoving.com/caleb-wood-essay)
- Jamie Wolfe: [Livin' in the Chaos Loop](https://mostlymoving.com/jamie-wolfe-essay)

Working with games and interactivity means thinking a lot about agency—what kind of agency will you give or deny your audience? Above, animators Jamie and Caleb talk about forces of **chaos** and **control** in relation to their practices. Take inspiration from Jamie and/or Caleb to formulate **at least three statements (number them!)** that explore how you feel about chaos and control in relation to your interactive practice.

### PART 2: GROUP MEDIA RESPONSE

**In groups of 2~3**, spend at least **30 minutes** with **any TWO (2)** of the following projects: [**LINK TO READING/MEDIA 1 LIST**](https://docs.google.com/spreadsheets/d/1bxmhYjV7zo1lLmPvBTt7lpUcrBbYTv12-mCrTIunIm8/edit?usp=sharing)

In what ways do the above interactive projects create meaning when they grant or deny you agency? 

Discuss among your group members, take notes, and submit a write-up of your collective response.

-->

## Reading / Media 2

## Reading / Media 3
