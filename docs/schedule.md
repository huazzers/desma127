# 📅 Schedule

<!--removes sidebar outline-->
<style>
    @media (min-width: 768px) {
        .col-md-9 {
            width: 100% !important;
        }
        
        .d-md-block {
        display: none !important;
        }
        
        #component-content{
            margin-left:0 !important;
        }
    }

    blockquote{
        margin: 0 0.5em;
    }

    table th:first-of-type {
        width: 10%;
    }
    table th:nth-of-type(2) {
        width: 45%;
    }
    table th:nth-of-type(3) {
        width: 45%;
    }

    table tr:nth-child(1)>td:nth-child(2), table tr:nth-child(8)>td:nth-child(2), table tr:nth-child(10)>td:nth-child(2){
        background-color:gray;
    }

</style>

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
    
    window.onload = function(e){
        var cell = document.getElementById('component-site-name');
        var caseId = cell.innerHTML;
        cell.innerHTML = '';
        var link = document.createElement('a');
        link.href = '../';
        link.appendChild(document.createTextNode(caseId));
        cell.appendChild(link);
    }
</script>

|  | Tuesday       | Thursday      |
| ------- | ------------- | ------------- |
| W0  | | **09/25**</br><p>Course Overview & Introductions</p><p>[Tech Setup](tech-setup.md)</p><p>Lecture: [What is Interactive Animation?](0-what-is-interactive-animation.md)</p><div class="assign"><p>▶️ ASSIGN:</p><ul><li>[Survey](https://forms.gle/eKqmPPXZrU3c5D4v6) (Due: W1 Tue, 09/30)</li><li>[Project 1](project-1.md) (Due: W4 Tue, 10/21)</li></ul></div>|
| W1  | **09/30**</br><div class="due"><p>📌 DUE: </p><ul><li>[Survey](https://forms.gle/eKqmPPXZrU3c5D4v6)</li></ul></div><p>Lecture: Key Principles of Interactive Animation</p><p>Tutorial: 2D Loops and Animation Basics</p><blockquote><p>Overview of basic animation concepts, including frame rates, keyframes, onion skinning, and the 12 principles of animation. Investigating how animation logic differs in films VS interactive projects.</p></blockquote><p>Studio Time (Start Animating Idle and Active Loops for Project 1)</p><div class="assign"><p>▶️ ASSIGN:</p><ul><li>[Reading/Media Response 1](reading-media.md/#reading-media-1) (Due: W2 Tue, 10/07)</li><li>[Project 1 Proposal](project-1.md/#deliverables) (Due: W2 Thu, 10/09)</li></ul></div> | **10/02**</br><p>Tutorial: Sprite Sheets and Animation States</p><blockquote><p>Animate Idle and Active Animation States for assets, bring sprite sheets into Unity.</p></blockquote><p>Studio Time (Animate Idle and Active States for assets, bring sprite sheets into Unity.)</p> |
| W2  | **10/07**</br><div class="due"><p>📌 DUE: </p><ul><li>[Reading/Media Response 1](reading-media.md/#reading-media-1)</li></ul></div><p>Tutorial: Intro to Unity and C# Scripts</p><blockquote><p>Conditional Statements, Point-and-click Interaction, Score-keeping.</p></blockquote><div class="assign"><p>▶️ ASSIGN:</p><ul><li>[Reading/Media Response 2](reading-media.md/#reading-media-2) (Due: W3 Tue, 10/14)</li></ul></div> | **10/09**</br><div class="due"><p>📌 DUE: </p><ul><li>[Project 1 Proposal](project-1.md/#deliverables)</li></ul></div><p>Tutorial: Rigging, Animating, and Interacting with 2D assets in Unity</p><blockquote><p>2D Puppet Rigging in Unity, 2D Navigation, Colliders, and Triggers.</p></blockquote>|
| W3  | **10/14**</br><div class="due"><p>📌 DUE:<p><ul><li>[Reading/Media Response 2](reading-media.md/#reading-media-2)</li></ul></div><p>Tutorial: Scene management, Animation Events, and "Game Manager" Scripts</p><blockquote><p>Creating and linking to new scenes and timeline events, Tips for Organizing your C# Scripts</p></blockquote> | **10/16**</br><p>Tutorial: Sound and Scene Design Tips, Building your Project</p><p>Studio Time: Bring your work and questions to class!<p>|
| W4  | **10/21**</br><div class="due"><p>📌 DUE: </p><ul><li>[Project 1](project-1.md)</li></ul></div><p>Project 1 Crit Day 1</p> | **10/23**</br><p>Project 1 Crit Day 2</p><div class="assign"><p>▶️ ASSIGN:</p><ul><li>[Reading/Media Response 3](reading-media.md/#reading-media-3) (Due: W6 Tue, 11/04)</li><li>[Project 2](project-2.md) (Due: W10 Tue, 12/02) and [Project 2 Proposal](project-2.md/#deliverables) (Due: W6 Thu, 11/06)</li></ul><!--<p><i>If you're new to Blender and 3D modelling, try out this exercise before next Tuesday: </i></p><ul><li>Easy Froggy Blender Tutorial</li></ul><p><i>Once you're done, send me your final render to earn extra credit!</i></p></div>--></div>|
| W5  | **10/28**</br><p>Lecture: 3D Interactive Animation and 3D Design in Virtual Environments</p><p>Tutorial: Intro to Blender Interface</p> | **10/30**</br><p>Tutorial: 3D Modelling and Rigging Workshop, 3D Unity Workflow</p><blockquote><p>We'll cover character modelling, UV Unwrapping, Texture Painting, 3D Rigging, and 3D Asset Imports into Unity (incl. multiple animations for the same model) -- so buckle up for a long tutorial day!</p></blockquote>|
| W6  | **11/04**</br><div class="due"><p>📌 DUE: </p><ul><li>[Reading/Media Response 3](reading-media.md/#reading-media-3)</li></ul></div><p>Tutorial: Interacting with 3D Assets in Unity</p><blockquote><p>3D Navigation, Ragdoll Physics, Character Controllers</p></blockquote> | **11/06**</br><div class="due"><p>📌 DUE: </p><ul><li>[Project 2 Proposal](project-2.md/#deliverables)</li></ul></div>Studio Time</blockquote>|
| W7  | **11/11**</br><p>No Class (Veterans Day holiday)</p> | **11/13**</br><p>Tutorial: Simple Custom Controller Workshop</p>|
| W8  | **11/18**</br><p>Tutorial: Extra tips and tricks (TBD)</p> | **11/20**</br><p>Tutorial: Post Processing, Effects</p><p>Studio Time: One-on-one meetings</p>|
| W9  | **11/25**</br><p>No Class (Thanksgiving holiday)</p> | **11/27**</br><p>Studio Time: One-on-one meetings</p>|
| W10  | **12/02**</br><div class="due"><p>📌 DUE: </p><ul><li>[Project 2](project-2.md)</li></ul></div><p>Project 2 Crit Day 1</p> | **12/04**</br><p>Project 2 Crit Day 2</p> |