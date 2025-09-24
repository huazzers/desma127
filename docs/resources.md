
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

# 🛠️ Resources and Tools

## Required Tools

### Equipment

You need a **3-button mouse with scrollwheel** for this course. 

<div class="assign"><p style="font-size:2.25em!important"><b>⚠️ ALWAYS BRING YOUR MOUSE TO CLASS! </b><img src="../img/your-mouse-that-you-didnt-bring-to-class.png" style="height:2em;"/></p></div>




### Software

> For more info on setting up Unity, Visual Studio / Code, and Blender, refer to the [**Tech Setup**](tech-setup.md) page.

<br>

We will be using the following programs:

- **Adobe Creative Apps** -- Install the latest version of **After Effects** and **Photoshop** onto your computer.
- **Blender** -- Install Blender on any devices you plan to use for your projects outside the classroom, just make sure you have **the same version as whatever's on the classroom computers**. Here is [an archive of their version releases](https://www.blender.org/download/releases/).
- **Unity** -- Please install [Unity Hub](https://unity.com/download) and get **any LTS version of Unity Editor between 2021~2023.** <br><div class="assign"><p style="font-size:2.25em!important"><b>⚠️ DO NOT USE UNITY 6!</b></p></div>
- **Visual Studio** -- Install Microsoft Visual Studio or Visual Studio Code, you should have the option to do this when installing Unity.
- **Mixamo** -- Mixamo is a useful, but limited, free in-browser auto-rigging application. We will use Mixamo for a quick exercise later in the quarter. All you need to do is [make an account with Mixamo](https://www.mixamo.com/#/) to use it in browser.

## Recommended Tools

### Drawing Tablets

While drawing tablets are not required for this class, they are essential for anyone who intends to incorporate digital drawing in their work now and in the future. 

We have several cintiq monitors in our classroom, and drawing tablets available for checkout at the 4th floor tech support office. **These are only available for classroom use.**

If you intend to purchase one for **personal use outside the classroom**, here are some recommendations: 

- Wacom tablets are the most reliable brand you can get. 
    - [**Wacom Intuos**](https://www.amazon.com/Wacom-Drawing-Software-Included-CTL4100/dp/B079HL9YSF/ref=sr_1_3?dchild=1&s=electronics&sr=1-3) is one of their cheapest options, it doesn't have a display. 
    - [**Wacom One**](https://www.wacom.com/en-us/products/pen-displays/wacom-one) is more costly and comes with a display. I personally use this one, too. It's a good investment if you like drawing digitally, and can double as a second monitor. 
- [**Huion H640P**](https://www.amazon.com/Inspiroy-H640P-Graphics-Battery-Free-Sensitivity/dp/B075T6MTJX/ref=sr_1_4?dchild=1&sr=8-4) is another good budget option. 
- Most surface or tablet devices, and even iPhones, can be paired with desktop PCs and Macs (depending on which OS they're compatible with.)
    - **iPads** can be paired with Mac using [the Sidecar feature](https://support.apple.com/en-us/102597), and be paired with PCs with [DuetDisplay](https://www.duetdisplay.com/use-ipad-as-second-monitor-for-mac-or-pc) for a subscription fee. 
    - **iPhones** can mirror your Mac desktop using [Yam Pad](https://www.yamdisplay.com/yampad/) and a USB connection to your Mac device. You can also get a stylus like [this](https://www.amazon.com/ORIbox-Stylus-Pen-Compatible-Smartphones/dp/B085FDR67C/ref=pb_allspark_session_sims_desktop_2?psc=1) to use your phone as a mini pen tablet. However, this option does not include pen pressure sensitivity. 

### Audio resources

- [**freesound.org**](https://freesound.org/) -- Audio database that can filter searches by license type. Login required for downloading files. Good sampling source for sound effects and music tracks.
- [**Audacity**](https://www.audacityteam.org/) -- free software for recording and editing audio; the version without Muse Hub should suffice for your purposes.
- [**Petaporon**](https://pixwlk.itch.io/petaporon) is a free minimalist piano roll sequencer you can use on the browser.  
- [**Lovely Composer**](https://1oogames.itch.io/lovely-composer) is a beginner-friendly music editor for $9 that is easy and fun to use. It comes with several chord templates and beat loops you can get started with, which is especially useful if you're completely new to music-making.

For more asset creation tools, there's also this **exhaustive list of cheap and free tools compiled by Everest Pipkin** -- [check out their section on sound and music-making tools](https://github.com/everestpipkin/tools-list?tab=readme-ov-file#sound--music).

### Animation resources

- [**The Animator's Survival Kit**](https://archive.org/details/TheAnimatorsSurvivalKitRichardWilliams/mode/2up) by Richard Williams is available on the Internet Archive for free! 
- [**Video to Riso Animation**](https://zinehug.com/Riso-Animation) with contact sheet templates provided
- [**Greenscreen Animals**](https://greenscreenanimals.com/footage) has video footage of various animals performing different actions. 

### CG resources

- [**Polycount Wiki**](http://wiki.polycount.com/) is a good reference for looking up terminology and formal principles related to 3D modelling. 
- [**RISD's Nature Lab Collection**](https://naturelab.risd.edu/collections/) includes links to their 3D models and images of animals, plants, human anatomy, and other natural specimens -- useful reference materials for drawing or modelling!


### C# scripting and Unity development

- **Unity documentation** -- [Scripting Reference](https://docs.unity3d.com/ScriptReference/index.html) and [Editor Manual](https://docs.unity3d.com/Manual/index.html).
- **Community Forums** -- [Stack Exchange](https://stackexchange.com/), [Unity Discussions](https://discussions.unity.com/).
- [**Learn C# in One Day and Learn it Well**](https://www.amazon.com/Learn-One-Day-Well-Hands/dp/1518800270) by Jamie Chan.
