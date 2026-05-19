## How to Make Your First Wario Ware Game




Have you ever played Wario Ware or any other really cool videogame? Have you ever thought of making your own version of the game? This tutorial will cover the basics of everything you need to know for making your first WarioWare videogame!

> If you already are familiar with Godot, feel free to jump through the tutorial. Have any questions while going through the tutorial? Feel free to dm us through slack at <b>@nonchalant ava (draws also)</b> and/or <b>@SuperCoolCodingGirlFNAF2014</b>

Now lets get started, shall we? C:




## Setting Up Godot
### What is Godot?
Godot is an open-source game engine where anyone can make 2D and 3D games in. In other words, it is a free place where we are going to make our game. For this tutorial, we're working with Godot 4. Try downloading the latest version.

### Downloading Godot
To download Godot, you need to consider the type of operating system your computer/laptop is using. Click the links below for the type you are using:
- [Download for macOS](https://godotengine.org/download/macos/)
- [Download for Windows](https://godotengine.org/download/windows/)
- [Download for Linux](https://godotengine.org/download/linux/)
- [Download for Android](https://godotengine.org/download/android/)

If the links above cannot be accessed or don't fit your operating system, navigate to https://godotengine.org/ and click "Download Latest"

![](/Screenshot%202026-05-16%20at%201.34.13 PM.png)

Click the blue button in the middle of the screen that reads "Godot Engine". Open the download and open the application. When you open Godot, it should look like this:

![](/godot-interface.webp)




## Setting up a GitHub Repository

### What is GitHub?
GitHub is a place in which we are going to share our files from Godot so our project can be submitted and reviewed for the Stardance Challenge.

### Downloading GitHub
Go to [github.com](https://github.com/). Click the "Enter your email" in the middle to sign up for GitHub and to create an account.
![](/Screenshot%202026-05-16%20at%201.46.07 PM.png)
Once you create your account or enter into your existing one, click the plus sign on the top right and click "New repository" to create a new repository.
![](/Github1.png)
Name it whatever you like. For me, I am going to name it "WarioWareGame." Make sure to make the repo public so the reviewers can see your work. Finish creating the repo by clicking "create repository"
![](/Github2.png)
Now we have to get our repository on our own computer! The fun part! Not really.



## Downloading GitHub Desktop
We need to download GitHub Desktop so we can actively save our work from our own computer. Go to [https://desktop.github.com/download/](https://desktop.github.com/download/). Click the download button that fits for your operating system.
![](/Screenshot%202026-05-16%20at%202.47.22 PM.png)
>As you work on this project, you will want to make hourly commits and pushes as you work so your work is constantly saving to your repo. So, keep this application open. What do I mean by **commiting** and **pushing**? I will explain that in a later section. C:



## Putting the GitHub project into our Local Repository
> P.S. If at any time you need help navigating through this part or get stuck, shoot us a dm through Slack **@SuperCoolCodingFNAF2014** or in the **#stardance** channel! <3

Now lets get started with clicking the "Set up in Desktop" button in the "Quick Setup" section in GitHub. This will prompt us to get the repository locally on our device. This will allow us to share our files onto GitHub.
![](/Github3.png)
Now you don't want to touch anything. Click "clone"
![](/Github4.png)
If you get taken to the GitHub Desktop, that is exactly where we want to be.

You will now want to click the "show in Finder" button or "show in FileManager" button. This will show you where your repository is. Keep track of this location. If you are on macOS, you can click **option + command + c** at the same time to copy the file address. If on Windows, you can **hold shift and right click the file to then select "Copy as path."** All these options save the file address, so we can later paste it into Godot.
![](/Github5.png)

Now navigate to Godot and create your first project! (YAY) Type your game's name into "Project Name:" and paste the address we had before into the project's path. You can paste by clicking **control + v** on Windows, or **command + v** on macOS. Then click "create".
![](/Screenshot%202026-05-16%20at%202.31.44 PM.png)
Now we can roll into the real fun stuff!</p>



## Creating the Start Menu

### What is a Start Menu?
A start menu is pretty much the place where the player will go to once they open the game. It will consist of a:
- Title
- Start Game Button
- Settings
- and a Quit Button

![](/Screenshot%202026-05-16%20at%204.29.03 PM.png)

### Creating the Title
Create a new "2D Scene." Name that new node "TitleScreen" so we can easily navigate through our nodes. What are **nodes**? Nodes are the building blocks of Godot when you build the game.

![](/Github6.png)
Click the + button near the top left corner of the screen. We want to add a new node that will act as the background image of our game. Search up "TextureRect" in the search when you click the "+". Name it "Background"


Now we want to change the texture of the TextureRect to the image we want the background to be. Click the "Background" node and go to the right of the screen. Click the file button next to "Texture." Upload any image you want.
![](/Github7.png)
To fit the image to the screen size, drag the image to the edge of the blue lines. The blue lines represent the size of the game screen.
![](/Github(1).png)
Now we want to display the title for our game. Create a new node by clicking the + again to make a new node and searching for the "RichTextLabel." Name it "Title." Drag the node on the background to position it where you want it on the screen. For me, I'm putting it in the almost top-center. Click the node, and on the right side of the screen, click the text box to type in the game's name.
![](/Godot.png)
Scroll down to the "Control" section and click "Theme Overrides" and then "Font Sizes." Check off "Normal" and change it to 108px. Can't see your text box? Try dragging out the textbox to change its size. Move the textbox to where you want it to be.

Now click "Constants" and click "Outline Size." Change it to 40. This adds a nice black outline to our text.
![](/Screenshot%202026-05-16%20at%205.22.59 PM.png)
Notice how the text seems cut off on the left? To fix that, go to "Layout" under "Control" and turn off "Clip Content." Now it should look like this:
![](/Screenshot%202026-05-16%20at%205.25.45 PM.png)

### Creating a Button
Now we have to add our "Start Game," "Settings," and "Quit" buttons.

Right click on the open space under the "Title" node. Search for "Button" and name it "Start." Click that node and go to the textbox on the right of the screen. Change what it says on the button to "Start Game." Drag the button to the desired size and move it to under the title, as shown below:
![](/Screenshot%202026-05-16%20at%205.29.39 PM.png)
Now we want to change the font size. Go to "Control" on the right then to "Theme Overrides" and then to "Font Sizes." Change the font size to 26px. Go to "Constants" and change the outline size to 14.
![](/Screenshot%202026-05-16%20at%205.47.31 PM.png)
Now we need to vertically align our three buttons. Click the + button on the top left to add a new node and search for "VBoxContainer." This container will help us align our buttons neatly in a vertical alignment. Drag the "Start" button into the container. It should look like this:
![](/Screenshot%202026-05-16%20at%205.50.31 PM.png)
Move the VBoxContainer to the middle. Drag out its height so more buttons can fit in the container.
![](/Screenshot%202026-05-16%20at%205.52.19 PM.png)
Click on the button node and click **control + d** to duplicate the buttons. Do this two times to have three buttons. Name the nodes "Start", "Settings", and "Quit." Go to each node's text box and change what they say to also either "Start", "Settings", and "Quit". Should look like this:
![](/Screenshot%202026-05-16%20at%206.00.41 PM.png)

### Saving the Project
There will be times where Godot crashes and all the progress for your project will be unsaved. Don't panic! I gotchu. To save a project, press **control + s.** A window will pop up asking you what to save the scene as. Create a new folder to save the scene in. Name the folder "Scenes." Save the scene in that folder and then click "Save."
![](/Screenshot%202026-05-16%20at%206.09.31 PM.png)
Make sure to do this often as you make your game. I don't want to see you crying over your game.

### Programming the Buttons
Now lets put some code into these buttons! The programming language that Godot uses is **GDScript**. It is specific towards Godot, but is relatively simple to learn. In my opinion, it is similar to Python.

We need to create a **script** for each node we want to add code to. A **script** is a set of written instructions for our nodes written in a programming language, specifically GDScript.

### Playtesting your Game



## Committing and Pushing to GitHub
Remember when I said that you have to constantly **push** and **commit** your game every hour? But what does that mean? To
**commit** means to save your work on your computer. To **push** means to actually bring those saved changes to GitHub. I know, it can sound confusing at first. Just remember there is just two buttons to click.

First, you want to navigate to your GitHub Desktop. You will see that some changes have been made. These changes are the changes you made to your Godot files. Every time you made a change to the game, GitHub Desktop will point it out. Now go to the bottom and click **commit**. Remember this saves your changes. A summary may be required before hitting commit. In that case, just type what you did, like "Created a Menu Screen."
![](/Screenshot%202026-05-16%20at%206.24.18 PM.png)
Now hit **push origin** or **publish branch**. This will put those saved changes from your project onto GitHub. And you're all good!
![](/Godot%20copy.png)
>Just remember to hit two buttons every hour you work on your project: **commit** and **push**. Try saying it 20 times fast!



## Creating the Level Scene
In the Level Scene, it will be the screen displayed between each minigame level. It will display what level you are on. The Screen will display:
- 5 pieces of Garlic representing the player's lives
- the Level Number
- and a Timer

![](/Screenshot%202026-05-18%20at%2012.22.00 PM.png)
    
### Creating a New Scene
Click the + next to the Title scene to create a new scene. Name it "level_scene."
![](/level1.png)
Click "2D Scene." Click the + and add in a "TextureRect" node and change the texture in the right side of the screen to the desired background. For me, I am going to keep it the same image.
![](/level2.png)
Resize the image to be the size of the screen. In order words, match it up to the blue lines again.

### Adding in the Garlic/Lives
In this game, the pieces of garlic will represent the lives of the player. Think of Minecraft and how the hearts in the game represented a player's health. The onions are similar to that concept.

We want the onions to be displayed in a horizontal alignment. So, click the 2D Scene node and click the + to search for a new node called "HBoxContainer."
![](/Screenshot%202026-05-16%20at%206.55.31 PM.png)
Click the HBoxContainer and the + button and search for a TextureRect node. This TextureRect will hold a picture of each onion/life. Rename the node to "Garlic." Rename the HBoxContainer to "GarlicContainer" to make it easier to navigate.
![](/Screenshot%202026-05-16%20at%206.56.00 PM.png)
Now click "Garlic" and press **control + d** to make 4 more pieces of garlic in the GarlicContainer. In total there should be 5. Can't see them? Try dragging out the length of the container. Rename each piece of garlic to "Garlic#" where # is the number of garlic it is. For example, the second garlic is "Garlic2"
![](/Screenshot%202026-05-16%20at%206.56.06 PM.png)
Drag and move the GarlicContainer to where you want it to be on the screen. For me, I am going to keep it near the top-center.
![](/Screenshot%202026-05-16%20at%206.56.57 PM%202.png)

### Adding in the Level Count & Timer
For the game, we need a piece of text saying what level number the player is on. We also need another piece of text stating how much time they have left.

Click the + button and add in two "RichTextLabel" nodes. Name one "Level" and the other "Timer."
![](/Screenshot%202026-05-16%20at%206.56.57 PM.png)
Click the "Level" node and go to the right of the screen. Change its text to "Level #" Do the same to the "Timer" node and change it to "0.0". You can move these nodes to wherever you want them on the screen. Also, go to Theme Overrides and then Colors to change the default color to black.
![](/Screenshot%202026-05-16%20at%206.58.58 PM.png)
Now lets change the font size. Click "Timer" and go to Control then to Theme Overrides and then to Font Sizes. Change the normal font size to 42px. Do the same to "Level."
![](/Screenshot%202026-05-16%20at%206.59.11 PM.png)
Drag out the size of the nodes' boxes on the screen to make sure the whole text is showing. Move them to where you seem fit.
![](/Screenshot%202026-05-16%20at%206.59.58 PM.png)

### Adding in the Garlic images
Change the texture for each piece of garlic to be a picture of garlic. If you don't want it to be garlic, that's okay. You can change it to a picture of a heart or anything else you would prefer. You change the picture by clicking each node and changing their texture on the right side of the screen.
![](/Screenshot%202026-05-18%20at%2011.54.28 AM.png)
After adding the new textures, you might have to rescale the nodes by dragging the corner of the box. You might have to also reposition the pieces of garlic.
![](/Screenshot%202026-05-18%20at%2011.54.33 AM.png)
Now we have 5 pieces of garlic. Yum!
![](/Screenshot%202026-05-18%20at%2011.54.55 AM.png)



## Programming the Level Scene
Now lets get started on the nerdy stuff. The timer, level count, and lives are not functional yet because they need code. So, lets get started on that.

### Programming the Timer
We need to create a **script** for each node we want to add code to. Remember, a **script** is a set of written instructions written in GDScript.

To add a script, click the 2D Scene and the paper scroll button above all your nodes. This adds a script attached to that 2D Scene.
![](/Screenshot%202026-05-18%20at%2011.55.13 AM.png)
Name it "timer_screen".
![](/Screenshot%202026-05-18%20at%2011.55.11 AM.png)