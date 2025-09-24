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

# How to Submit

## Important Notes

⚠️ **NAME YOUR SUBMISSION FILES CLEARLY WITH YOUR NAME AND PROJECT TITLE**, e.g. YourName_Project1.zip.

⚠️ **DO NOT SHOW THE UNITY EDITOR IN YOUR VISUAL DOCUMENTATION.** 

⚠️ **BUILD EARLY AND PLAY TEST YOUR BUILDS.** Some bugs will only reveal themselves in a build, so make sure to catch those in advance of the deadline. A broken game will affect your project grade. 


---

## Submission Checklist

**<u>Before class on the day of the project deadline</u>**

The following items should be handed in through the project submission form **before class starts**: 

> - **Project Title**
> - **Project Statement** -- can be descriptive of the piece, but should mostly focus on your motivation for making it.
> - **Instructions for interactivity** -- which buttons do I press?
> - **Project build for WINDOWS**, zipped with the folder and .dll file that Unity will export along with the .exe file.
> - **Exported Unity package**, with the file extension (.unitypackage).


<br>

**<u>By 11:59PM on the day of the project deadline:</u>**

Submit the following **visual documentation** of your project in the same submission form:

<mark class="assign">⚠️ **DO NOT SHOW THE UNITY EDITOR IN YOUR VISUAL DOCUMENTATION.**</mark>

> - **at least ONE animated GIF** of your project in motion, roughly 600 pixels wide, ideally under 5MB in size.
> - **at least TWO stills** from your project (1920x1080).
> - **(Optional) Recording of gameplay.** Roughly 60 seconds, long enough to demonstrate how your game is played (1920x1080, mp4/h.264)


<br>

---

## Tools for Visual Documentation

### Animated GIFs

Animated GIFs are durable and easy to view (though not always small in size). In this course we will use animated GIFs as a quasi-archival format for animated visual material. Preferably, they should be 600 pixels wide and under 5MB in file size.

I personally use and recommend [ScreenToGif](https://www.screentogif.com/), which is a good tool for quickly making a gif. Photoshop, Premiere, AfterEffects, or other video editors can also export gifs. You may also find the following free tools helpful:

- [EzGif.com](https://ezgif.com/) is an online GIF maker, editor, and compressor. Great for reducing the file size of GIFs.
- [LICEcap](https://www.cockos.com/licecap/) is a badly-named free OSX app which can capture an area of your screen and save it directly to an animated GIF.
- [Online-convert.com](https://www.online-convert.com/) offers a browser tool for converting videos into GIFs.

<br>

### Screenshots and Screen Recordings

**Make a build first and run it full screen** to capture images and video of your project. 

For screen recordings, [OBS](https://obsproject.com/) works very well. 

You may also use the [Unity Recorder](https://learn.unity.com/tutorial/working-with-unity-recorder) to capture single frames and videos from within the Unity Editor.

<br>

#### Built-in OS screenshot shortcuts:

##### Windows

To take a screenshot and automatically save the file, press the **Windows key + PrtScn**. Your screen will go dim and a screenshot of your entire screen will save to the **Pictures > Screenshots folder**.

Also consider the snipping tool, which is a convenient way to capture a portion of your screen.

<br>

##### Mac

1. To take a screenshot, press **Shift + Command + 3**.
2. If you see a thumbnail in the corner of your screen, click it to edit the screenshot. Or wait for the screenshot to save to your desktop.

By default, screenshots save to your **desktop** with the name ”Screen Shot [date] at [time].png.”

<br>

---

## How to export projects from Unity

Before we export anything...

### Project / Player Settings for Unity Build

<!---->

Go to **Edit > Project Settings > Select the Player tab**. 

![](./img/project-settings.jpg)

<br>

Here's some settings you may customise:

- **Product Name** - Set this to your project title. This will be the name of the executable file (.exe). 
- **Default Icon and Cursor** - Set the executable file icon and in-game cursor. 
- **Resolution and Presentation** - You may calibrate whether your game application runs in the background, and whether it opens in fullscreen or windowed view.

<br>

### Building your project

Start by opening the build settings under **File > Build Settings**.

![](./img/build_settings_1.gif)

<br>

Add all the scenes you want to include in your project by clicking and dragging them from your assets folder to “Scenes in Build” (also remove any scenes you don’t want to include). The topmost scene in this list will be the first to play when starting the game.

![](./img/build_settings_2.gif)

<br>

Create a Windows build by changing Target Platform to “Windows” and clicking build.

![](./img/build_settings_3.gif)

<br>

After the build has finished, locate the folder containing all the files and folders that Unity created. **The build needs all these folders, exes, and dlls to run properly.**

![](./img/Unity%20Build%20zip.png)

<br>

Rename this folder as **"YourName_Project123_Build"**, then compress it into a zipped folder. You will upload this .zip folder on itch.io and submit it for documentation.

<br>


### Unity Packages

> Read the official documentation for [exporting and importing Unity packages](https://docs.unity3d.com/Manual/AssetPackagesCreate.html).

Rather than creating a zip file of your entire Unity project folder, you can save a lot of time (and space) by exporting only the assets for the scenes, materials, prefabs, etc. that you want to share. This is called exporting an asset package.

<br>

#### Exporting Unity Packages

You have two options:

- Find your scene file in the Project tab, right click the scene, and click “Export Package…” <br> ![](./img/export-package-1.gif) <br><br>
- OR Click **Assets > Export Package…** <br> ![](./img/export-package-2.gif)

<br>

In the window that opens, de-select any assets that you don’t want to include. Be careful that you don’t exclude anything required to run your scene. If you only had your scene selected when clicking **Export Package…**, the window will only display the assets directly used in that scene. You can select entire folders, or even the top level Assets folder to bring up more assets to include in the export.

Select **None**, then click **Include dependencies** box to include all assets used inside your scene. Finally, click **Export…** to save your unitypackage file.

Name this Unity Package "YourName_Project123.unitypackage"

![](./img/export-package-3.gif)

<br>

#### Importing Unity Packages

To import a package into another project, double click the “.unitypackage” file with a project open and an import window will appear.

![](./img/import-package-1.gif)

<br>

You can also click **Assets > Import Package > Custom Package…** to select the unitypackage file via explorer/finder.

Select the assets you want to import and click **Import**.