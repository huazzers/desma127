
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

# Tech Setup

## Setting up Unity and Visual Studio / Code

1. Create a [Unity ID](https://login.unity.com/en/sign-up) if you don't already have one, and download **Unity Hub**: [https://unity.com/download](https://unity.com/download)  

2. Open Unity Hub, and download **any version of Unity Editor (2021~2023) with long term support (LTS)**<br><div class="assign"><p style="font-size:2.5em!important"><b>⚠️ DO NOT USE UNITY 6!</b></p></div>

3. When downloading the Unity Editor, make sure to include the following modules (in check boxes)

    * ✅ **Microsoft Visual Studio Community**   
        (\*only available on WINDOWS)

        * If prompted to run the Visual Studio Installer, make sure that “Game Development with Unity” is checked under the Workloads tab.

        ![](./img/vs-installer-unity.jpg)

        * **If you’re using a Mac device:**  
        Because Visual Studio for Mac is no longer supported, you’ll need to download [Visual Studio Code](https://code.visualstudio.com/) instead.

        Next, install the Unity for Visual Studio Code extension (published by Microsoft) from the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=visualstudiotoolsforunity.vstuc), or the [Extensions Marketplace](https://code.visualstudio.com/docs/configure/extensions/extension-marketplace) inside Visual Studio Code.

    * ✅ **Windows Build Support (IL2CPP or Mono)**

    * ✅ **Mac Build Support (IL2CPP or Mono)**

4. In Unity Hub, **activate a free personal Unity license.**

    ![](./img/activate-personal-license.gif)

5. **Make a New Unity Project.**

    In Unity Hub, go to Projects \> New Project \> Select your editor version at the dropdown field above \> Select Universal 2D (To start, we will use the Universal Render Pipeline and create a 2D Unity Project.) 

    All Unity projects are stored locally as a folder on your computer. Select a name (e.g. “InteractiveAnimationProject1”) and location for your project folder.

    We’ll leave “Connect to Unity Cloud” and “Use Unity Version Control” unchecked for now. 

    Then click “Create Project.” 

6. **Set up Unity for Visual Studio / Code integration**

    Open up your newly created Unity project. In the Unity Editor, go to Windows \> Package Manager \> Make sure that Visual Studio Editor package (version 2.0.20 and above) has been installed on your project. 

    Then, go to Edit \> Preferences \> External Tools \> Select your External Script Editor as either “Visual Studio” or “Visual Studio Code”. This will be the default program that runs when you try to open up a script in Unity. 

### Intellisense for Unity C&#35;

![](./img/intellisense.gif)

Intellisense is a useful **auto-complete feature** that will give a dropdown list of suggestions for your code as you're typing. 

I recommend getting this working on your scripting program, because it will make the process of understanding C# a lot more assisted and easier to navigate. It is also helpful for referencing variables and functions across multiple scripts in your projects.

If you're not getting any dropdown options when writing your code, try troubleshooting your Intellisense feature -- here's some resources you may start from: 

- **For Visual Studio Code:** <br> [Stack Overflow: How to get intellisense in Visual Studio Code for Unity functions names?](https://stackoverflow.com/questions/52189426/how-to-get-intellisense-in-visual-studio-code-for-unity-functions-names)
- **For Visual Studio:** <br> [Fixing Visual Studio’s IntelliSense (auto-complete) in Unity](https://blog.terresquall.com/2020/11/fixing-visual-studios-intellisense-autocomplete-in-unity/)


---

## Setting up Blender

On your own laptop or desktop, install the same version of Blender that's on the classroom computers. 

> Here is an archive of all released versions of Blender: [download.blender.org/release](https://download.blender.org/release/)

<br>

For a better experience in Blender, follow the instructions below to calibrate your Blender preferences accordingly: 

<br>

### Input Preferences

Make the most out of your 3-button mouse by activating their shortcut options!

- Go to **Edit > Preferences > Input**
- Toggle on **Emulate 3 Button Mouse**

<br>

### Keymap Preferences

Switch object interaction modes and viewport shading modes using hotkeys.

- Go to **Edit > Preferences > Keymap**
- Under 3D View, toggle on **"Tab for Pie Menu"** and **"Extra Shading Pie Menu Items"**.

<br>

### Extra Mesh Objects

Activate this add-on to view more mesh options. The Round Cube mesh is particularly useful when cube modelling.  

- Go to **Edit > Preferences > Add-ons**
- Toggle on **"Extra Mesh Objects"** (*or "Add Mesh: Extra Objects" in version 3.x*)

<br>

### Loop Tools 

If you have Blender 4.x:

- Go to **Edit > Preferences > Get Extensions**
- Click **"Allow Online Access"** to connect to the network if prompted -- you can turn this off later in the System tab, under **Network**.
- Search for **"LoopTools"** > click **Install**.

<br>

If you have Blender 3.x:

- Go to **Edit > Preferences > Add-ons**
- Toggle on **"Mesh: LoopTools"**.

<br>

### Lazy Viewport plugin

*(Optional, depends on preference!)*

By default, pressing Blender's transform hotkeys (scale, move, rotate) will automatically perform the tool's transform action. 

If you're not a fan of this feature, and want the hotkeys to simply switch to the tool *without* performing the transform action, I recommend downloading this **Lazy Viewport** add-on: [https://github.com/cgfasttrack/lazyviewport](https://github.com/cgfasttrack/lazyviewport)

<br>

- On the github page, click the green button **"<> Code" > Download ZIP**. <br><br><img src="../img/techsetup_lazyviewport.jpg" width = "80%"><br><br>
- **Extract the .zip folder**. There should be a **python file (.py)** inside the extracted folder "lazyviewport.py".<br><br><img src="../img/lazyviewportpy.jpg"><br><br>
- In Blender, go to **Edit > Preferences > Add-ons**.
- Click the **dropdown arrow** at the top right of the menu window **> Install from Disk**<br><blockquote><p>If you're on Blender version 3.x, click the "Install" button at the top right corner.</p></blockquote><br><img src="../img/installAddons.jpg" width = "80%"><br><br>
- Locate and select the **"lazyviewport.py"** file, then click **"Install from Disk"**.
- Make sure the "Lazy Viewport" module is toggled on in your Add-on settings.<br><br><img src="../img/lazyviewportaddon.jpg"><br><br>
