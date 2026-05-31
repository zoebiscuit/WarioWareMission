# How to Make Your First WarioWare-style Game
![](https://cdn.hackclub.com/019e7531-d4f8-7ae2-8822-d79ce11875e8/wario-ware_style_game_3_.png)

Have you ever played Wario Ware or any other really cool videogame? Have you ever thought of making your own version of the game? This tutorial will cover the basics of everything you need to know for making your first WarioWare videogame!

> If you already are familiar with Godot, feel free to jump through the tutorial. Have any questions while going through the tutorial? Feel free to dm us through slack at <b>@nonchalant ava (draws also)</b> and/or <b>@SuperCoolCodingGirlFNAF2014</b>

Now lets get started, shall we? C:

# Setting Up Godot
> ### What is Godot?
> Godot is an open-source game engine where anyone can make 2D and 3D games in. In other words, it is a free place where we are going to make our game. For this tutorial, we're working with Godot 4. Try downloading the latest version.

### Downloading Godot
To download Godot, you need to consider the type of operating system your computer/laptop is using. Click the links below for the type you are using:
- [Download for macOS](https://godotengine.org/download/macos/)
- [Download for Windows](https://godotengine.org/download/windows/)
- [Download for Linux](https://godotengine.org/download/linux/)
- [Download for Android](https://godotengine.org/download/android/)

If the links above cannot be accessed or don't fit your operating system, navigate to https://godotengine.org/ and click "Download Latest"

![](https://cdn.hackclub.com/019e74bf-da12-762f-b3be-c89479f9fbbf/image.png)

Click the blue button in the middle of the screen that reads "Godot Engine". Open the download and open the application. When you open Godot, it should look like this:

![](https://cdn.hackclub.com/019e74c4-8b1c-7604-ae3d-4fcc4fbc1162/image.png)

# Setting up a GitHub Repository
> ### What is GitHub?
> GitHub is a place in which we are going to share our files from Godot so our project can be submitted and reviewed for the Stardance Challenge.

### Downloading GitHub
Go to [github.com](https://github.com/). Click the "Enter your email" in the middle to sign up for GitHub and to create an account.

![](https://cdn.hackclub.com/019e74c6-14f2-787d-a63f-2b130fc75977/image.png)

Once you create your account or enter into your existing one, click the plus sign on the top right and click "New repository" to create a new repository.

![](https://cdn.hackclub.com/019e74c6-223d-7956-8a30-49178b1caeda/image.png)

Name it whatever you like. For me, I am going to name it "WarioWareGame." Make sure to make the repo public so the reviewers can see your work. Finish creating the repo by clicking "create repository"

![](https://cdn.hackclub.com/019e74c6-4009-751f-9a22-dcbf7fb1e89e/image.png)

Now we have to get our repository on our own computer!

# Downloading GitHub Desktop
> If you struggle to download GitHub Desktop on your device, I recommend checking out [this resource](https://beta.stardance.hackclub.com/guides/github_repository) for alternatives!

We need to download GitHub Desktop so we can actively save our work from our own computer. Go to [https://desktop.github.com/download/](https://desktop.github.com/download/). Click the download button that fits for your operating system.

![](https://cdn.hackclub.com/019e74c7-ff35-7e38-bc1a-b50940fb320b/image.png)

>As you work on this project, you will want to make hourly commits and pushes as you work so your work is constantly saving to your repo. So, keep this application open. What do I mean by **commiting** and **pushing**? I will explain that in a later section. C:

# Putting the GitHub project into our Local Repository
> P.S. If at any time you need help navigating through this part or get stuck, shoot us a dm through Slack **@SuperCoolCodingFNAF2014** or in the **#stardance** channel! <3

Now lets get started with clicking the "Set up in Desktop" button in the "Quick Setup" section in GitHub. This will prompt us to get the repository locally on our device. This will allow us to share our files onto GitHub.

![](https://cdn.hackclub.com/019e74c8-a238-798e-8d0e-4d1878739fce/image.png)

Now you don't want to touch anything. Click "clone"

![](https://cdn.hackclub.com/019e74c9-2227-7124-aa4f-aaed218f079f/image.png)

If you get taken to the GitHub Desktop, that is exactly where we want to be.

You will now want to click the "show in Finder" button or "show in FileManager" button. This will show you where your repository is. Keep track of this location. If you are on macOS, you can click **option + command + c** at the same time to copy the file address. If on Windows, you can **hold shift and right click the file to then select "Copy as path."** All these options save the file address, so we can later paste it into Godot.

![](https://cdn.hackclub.com/019e74ca-1f8a-7025-960d-71acb77cd084/image.png)

Now navigate to Godot and create your first project! (YAY) Type your game's name into "Project Name:" and paste the address we had before into the project's path. You can paste by clicking **control + v** on Windows, or **command + v** on macOS. Then click "create".

![](https://cdn.hackclub.com/019e74ca-3701-7242-8a83-ecf7c72b11e9/image.png)

Now we can roll into the real fun stuff!

# Creating the Start Menu
> ### What is a Start Menu?
> A start menu is pretty much the place where the player will go to once they open the game. It will consist of a:
> - Title
> - Start Game Button
> - Settings
> - and a Quit Button
>
> ![](https://cdn.hackclub.com/019e74cb-b1ae-7729-9b1e-2748791ddd2a/image.png)

### Creating the Title
Create a new "2D Scene." Name that new node "TitleScreen" so we can easily navigate through our nodes. What are **nodes**? Nodes are the building blocks of Godot when you build the game.

![](https://cdn.hackclub.com/019e74cb-db55-7dac-ac10-14cbe805d38d/image.png)

Click the + button near the top left corner of the screen. We want to add a new node that will act as the background image of our game. Search up "TextureRect" in the search when you click the "+". Name it "Background"


Now we want to change the texture of the TextureRect to the image we want the background to be. Click the "Background" node and go to the right of the screen. Click the file button next to "Texture." Upload any image you want.

![](https://cdn.hackclub.com/019e74cb-f804-77f9-8d5b-b988c372f4e3/image.png)

To fit the image to the screen size, drag the image to the edge of the blue lines with the scale tool. The blue lines represent the size of the game screen.

![](https://cdn.hackclub.com/019e74cc-0900-759e-ae16-3ca1ca7feb79/image.png)

Now we want to display the title for our game. Create a new node by clicking the + again to make a new node and searching for the "RichTextLabel." Name it "Title." Drag the node on the background to position it where you want it on the screen. For me, I'm putting it in the almost top-center. Click the node, and on the right side of the screen, click the text box to type in the game's name.

![](https://cdn.hackclub.com/019e74cc-1b08-7a2e-b619-de1d7cc49d26/image.png)

Scroll down to the "Control" section and click "Theme Overrides" and then "Font Sizes." Check off "Normal" and change it to 108px. Can't see your text box? Try dragging out the textbox to change its size. Move the textbox to where you want it to be.

Now click "Constants" and click "Outline Size." Change it to 40. This adds a nice black outline to our text.

![](https://cdn.hackclub.com/019e74cc-37fc-7e47-a58a-1035f55ec201/image.png)

Notice how the text seems cut off on the left? To fix that, go to "Layout" under "Control" and turn off "Clip Content." Now it should look like this:

![](https://cdn.hackclub.com/019e74cc-48ff-7637-ac91-6c5cd002b416/image.png)

### Creating a Button
Now we have to add our "Start Game," "Settings," and "Quit" buttons.

Add a new node with the plus button. Search for "Button" and name it "Start." Click that node and go to the textbox on the right of the screen. Change what it says on the button to "Start Game." Drag the button to the desired size and move it to under the title, as shown below:

![](https://cdn.hackclub.com/019e74cc-5b87-71bb-8614-2291cc7e258c/image.png)

Now we want to change the font size. Go to "Control" on the right then to "Theme Overrides" and then to "Font Sizes." Change the font size to 26px. Go to "Constants" and change the outline size to 14.

![](https://cdn.hackclub.com/019e74cc-7255-722d-9d3d-5d57a83765cc/image.png)

Now we need to vertically align our three buttons. Click the + button on the top left to add a new node and search for "VBoxContainer." This container will help us align our buttons neatly in a vertical alignment. Drag the "Start" button into the container. It should look like this:

![](https://cdn.hackclub.com/019e74cc-7989-7575-bbd9-e338c43a30b4/image.png)

Move the VBoxContainer to the middle. Drag out its height so more buttons can fit in the container.

![](https://cdn.hackclub.com/019e74cc-9a89-72e1-ba72-ba6feb43de59/image.png)

Click on the button node and click **control + d** to duplicate the buttons. Do this two times to have three buttons. Name the nodes "Start", "Settings", and "Quit." Go to each node's text box and change what they say to also either "Start", "Settings", and "Quit". Should look like this:

![](https://cdn.hackclub.com/019e74cc-b179-77bb-bf09-3dffc89707f2/image.png)

### Saving the Project
There will be times where Godot crashes and all the progress for your project will be unsaved. Don't panic! I gotchu. To save a project, press **control + s.** A window will pop up asking you what to save the scene as. Create a new folder to save the scene in. Name the folder "Scenes." Save the scene in that folder and then click "Save."

![](https://cdn.hackclub.com/019e74cc-d082-7945-b4db-d72c60806137/image.png)

Make sure to do this often as you make your game. I don't want to see you crying over your game.

### Programming the Buttons
Now lets put some code into these buttons! The programming language that Godot uses is **GDScript**. It is specific towards Godot, but is relatively simple to learn. In my opinion, it is similar to Python.

> We need to create a **script** for each node we want to add code to. A **script** is a set of written instructions for our nodes written in a programming language, specifically GDScript.

Go to the "TitleScreen" node and add a script by clicking the paper scroll button. Save that new script.

![](https://cdn.hackclub.com/019e757e-ecdd-7e42-8cb9-15fb10b1f097/14.png)

Click the "Start" button node on the left. Go to the right of the screen and click "Signals" and double click "pressed()" 

![](https://cdn.hackclub.com/019e757e-efdb-7c41-8eeb-371322c56d5e/15.png)
![](https://cdn.hackclub.com/019e757e-f285-7e07-92eb-402157953806/16.png)

> What are **signals**? Signals track when changes are created so we can create code to make our game respond to it. In this case, we're making the game react to the player pressing the button.

Connect the Script to the "TitleScreen" node, not the button. To make sure its connected, make sure TitleScreen is highlighted.

![](https://cdn.hackclub.com/019e757e-f54f-7d2f-96bf-aa9a3a34adc6/17.png)

It should have navigated you to the "TitleScreen" node's script. 

![](https://cdn.hackclub.com/019e757d-1669-71ef-805c-9dda5018136c/screenshot_2026-05-29_at_4.46.03___pm.png)

Under the "func _on_button_pressed() -> void:" we want to add "get_tree().change_scene_to_file("???")" where ??? is the location of the scene in your local computer. The specific location might be different for other people. It should look like this:

	func _on_button_pressed() -> void:
		get_tree().change_scene_to_file("res://node_2d.tscn")



> ### Playtesting your Game
> While you make your game, you want to test your game throughout. We do this to catch any errors. How do you do that? Simple. Click the play button on the top of the screen.
> ![](https://cdn.hackclub.com/019e7588-42ed-7d4a-b39d-e57c23397c83/godot.png)

# Committing and Pushing to GitHub
>Remember when I said that you have to constantly **push** and **commit** your game every hour? But what does that mean? To **commit** means to save your work on your computer. To **push** means to actually bring those saved changes to GitHub. I know, it can sound confusing at first. Just remember there is just two buttons to click.

First, you want to navigate to your GitHub Desktop. You will see that some changes have been made. These changes are the changes you made to your Godot files. Every time you made a change to the game, GitHub Desktop will point it out. Now go to the bottom and click **commit**. Remember this saves your changes. A summary may be required before hitting commit. In that case, just type what you did, like "Created a Menu Screen."

![](https://cdn.hackclub.com/019e74e7-91ca-791c-a12a-5475dca9ebd9/image.png)

Now hit **push origin** or **publish branch**. This will put those saved changes from your project onto GitHub. And you're all good!

![](https://cdn.hackclub.com/019e74e7-fcda-74ef-851e-a66fd3cfdc44/image.png)

>Just remember to hit two buttons every hour you work on your project: **commit** and **push**. Try saying it 20 times fast!

# Creating the Level Scene
> In the Level Scene, it will be the screen displayed between each minigame level. It will display what level you are on. The Screen will display:
> - 5 pieces of Garlic representing the player's lives
> - the Level Number
> - and a Timer
>
> ![](https://cdn.hackclub.com/019e74e8-f458-73e3-ae7b-31b0832120aa/image.png)
    
### Creating a New Scene
Click the + next to the Title scene to create a new scene. Name it "level_scene."

![](https://cdn.hackclub.com/019e74e9-0e64-79bb-9e7c-02e9643f8f41/image.png)

Click "2D Scene." Click the + and add in a "TextureRect" node and change the texture in the right side of the screen to the desired background. For me, I am going to keep it the same image.

![](https://cdn.hackclub.com/019e74e9-1962-7066-9b3e-5cf8dee393e8/image.png)

Resize the image to be the size of the screen. In order words, match it up to the blue lines again.

### Adding in the Garlic/Lives
In this game, the pieces of garlic will represent the lives of the player. Think of Minecraft and how the hearts in the game represented a player's health. The garlic are similar to that concept.

We want the garlic to be displayed in a horizontal alignment. So, click the 2D Scene node and click the + to search for a new node called "HBoxContainer."

![](https://cdn.hackclub.com/019e74e9-324b-7754-94f9-9354ce9af828/image.png)

Click the HBoxContainer and the + button and search for a TextureRect node. This TextureRect will hold a picture of each garlic/life. For now, change the texture to the icon.svg, which is the Godot logo. Rename the node to "Garlic." Rename the HBoxContainer to "GarlicContainer" to make it easier to navigate.

![](https://cdn.hackclub.com/019e74e9-446f-7481-a23e-d4cd962dfe05/image.png)

Now click "Garlic" and press **control + d** to make 4 more pieces of garlic in the GarlicContainer. In total there should be 5. Can't see them? Try dragging out the length of the container. Rename each piece of garlic to "Garlic#" where # is the number of garlic it is. For example, the second garlic is "Garlic2"

![](https://cdn.hackclub.com/019e74e9-5901-779c-bf98-366f8ec464e4/image.png)

Drag and move the GarlicContainer to where you want it to be on the screen. For me, I am going to keep it near the top-center.

![](https://cdn.hackclub.com/019e74e9-6c2f-7b42-bf3d-c7c35776fd7f/image.png)

### Adding in the Level Count & Timer
For the game, we need a piece of text saying what level number the player is on. We also need another piece of text stating how much time they have left.

Click the + button and add in two "RichTextLabel" nodes. Name one "Level" and the other "Timer."

![](https://cdn.hackclub.com/019e74e9-7594-7cf0-81af-88149c486c46/image.png)

Click the "Level" node and go to the right of the screen. Change its text to "Level #" Do the same to the "Timer" node and change it to "0.0". You can move these nodes to wherever you want them on the screen. Also, go to Theme Overrides and then Colors to change the default color to black.

![](https://cdn.hackclub.com/019e74e9-9380-71c5-a80c-b16f9601ead3/image.png)

Now lets change the font size. Click "Timer" and go to Control then to Theme Overrides and then to Font Sizes. Change the normal font size to 42px. Do the same to "Level."

![](https://cdn.hackclub.com/019e74e9-a161-7e78-b1a0-80b4a420a08b/image.png)

Drag out the size of the nodes' boxes on the screen to make sure the whole text is showing. Move them to where you seem fit.

![](https://cdn.hackclub.com/019e74e9-bde0-7ada-a6e6-6b7194979d74/image.png)

### Adding in the Garlic images
Change the texture for each piece of garlic to be a picture of garlic. If you don't want it to be garlic, that's okay. You can change it to a picture of a heart or anything else you would prefer. You change the picture by clicking each node and changing their texture on the right side of the screen.

![](https://cdn.hackclub.com/019e74e9-ce4c-7c66-ae1a-84ca9a80c7ed/image.png)

After adding the new textures, you might have to rescale the nodes by dragging the corner of the box. You might have to also reposition the pieces of garlic.

![](https://cdn.hackclub.com/019e74e9-e296-7bda-a56d-f6e0b2ec8b90/image.png)

Now we have 5 pieces of garlic. Yum!

![](https://cdn.hackclub.com/019e74e9-f6ec-7461-84e0-29d65955b007/image.png)

# Creating a Platformer Minigame
> You are going to be making a minigame where you will have to collect a total of 3 garlics around a map on a platformer. We will need:
> - A Moving Player
> - A Platform
> - Garlic Object(s)
> - and barriers
>
> So, lets get right on it!

![](https://cdn.hackclub.com/019e76f2-9fff-75a0-a212-942231b96f2e/ezgif-5b392a49736051f9.gif)

## Creating the Player

Make a new scene called "Player." Change its type to "CharacterBody2D" by right clicking the "Player" node.

![](https://cdn.hackclub.com/019e76b9-ff6e-7bd4-a528-9931b7442dc2/image.png)

Add a node called "Sprite2D" and another called "CollisionShape2D"

![](https://cdn.hackclub.com/019e76ba-5a07-7fb6-a8bd-257df697d31b/image.png)

Change the CollisionShape2D's shape to CircleShape.

![](https://cdn.hackclub.com/019e76ba-5cd8-715e-b31d-f2face96333d/image.png)

Change Sprite2D's texture to the image of the character you want. For me, I am doing a pixelated version of Wario I got from online.

Resize the CollisionShape2D to cover the whole player by dragging the red dot on the circle with your mouse.

![](https://cdn.hackclub.com/019e76ba-5fc7-7f46-af44-20e28d2eb9b1/image.png)

Create a script for the "Player" node. Make sure its template is "CharacterBody2D: Basic Movement"

![](https://cdn.hackclub.com/019e76bd-7d93-7c3b-ac66-de8780eac4b7/screenshot_2026-05-29_at_10.36.16___pm.png)

## Creating the Platform

Make a new 2D scene. Name it "minigame_1." Add a StaticBody2D node. To that node, add a ColorRect node and a CollisionShape2D node. Should look like the image below.

![](https://cdn.hackclub.com/019e76d9-5f49-76c8-8825-1e3330066e03/screenshot_2026-05-29_at_11.06.30___pm.png)

Change the color of the ColorRect node to the color you want it to be. The ColorRect will represent the barrier. Go to the CollisionShape2D and change its shape to rectangle.

![](https://cdn.hackclub.com/019e76c6-a411-7d03-9d6e-432b21370300/screenshot_2026-05-29_at_10.46.17___pm.png)

Stretch the CollisionShape2D to cover the whole ColorRect. Just like we did to the player previously.

![](https://cdn.hackclub.com/019e76d9-61c0-7071-8807-6a5095b5766b/screenshot_2026-05-29_at_11.06.47___pm.png)

Move and drag the CollisionShape2D to be on the bottom of the screen. Think of it as the ground of the game in which the player will stand on. Make the ColorRect match up to it as well, so they are in the same position and in the same shape. 

![](https://cdn.hackclub.com/019e76e5-8616-7538-bb38-90377b6c523f/screenshot_2026-05-29_at_11.20.01___pm.png)

Add a TextureRect to the 2D Scene. This will act as the background. Change its texture to its desired background and resize it to fit the screen. Drag the TextureRect node to be behind the StaticBody2D node so the background does not cover those nodes. It should look like this:

![](https://cdn.hackclub.com/019e76e8-cc92-713a-bbd9-9512eda6b412/screenshot_2026-05-29_at_11.23.36___pm.png)

Name the TextureRect "Background" so we can navigate through our nodes easily. Add a "Parallex2D" node to our 2D scene. Add our "Background" node to it. The "Parallex2D" node is responsible for animating the background into having a scrolling effect, so rename it to "ScrollingBackground." This is optional.

![](https://cdn.hackclub.com/019e770c-5da8-7492-9e83-f0b0f9d622dd/screenshot_2026-05-30_at_12.02.26___am.png)

For the Parallex2D node, go to the right of the screen and click the "Repeat" menu. Change the Repeat Size x to 1000.0. As you can notice it stretches the background image to the right. Now, Change its AutoScroll x setting to 100.0.

![](https://cdn.hackclub.com/019e7a1b-d2e1-7aef-afca-ac8c96888e22/screenshot_2026-05-30_at_2.18.13___pm.png)

> ## How come my screen can't be full screen? Let's fix that!
> ![](https://cdn.hackclub.com/019e7a1e-05f3-7026-8ee1-7c1e0ec56fb1/screenshot_2026-05-30_at_2.20.39___pm.png)
> Go to the Project menu on the top of your screen and go to your Project's settings.
> ![](https://cdn.hackclub.com/019e7a20-9fee-7608-a02a-b8ace602a544/screenshot_2026-05-30_at_2.21.22___pm.png)
> Then go to Display and then Window. Change the mode to "viewport."
> ![](https://cdn.hackclub.com/019e7a20-a1fa-7624-8ae3-5d2dfc40b776/godot_1_.png)
> Now test your game and change the screen to be able to "Stretch to Fit" at the top of your screen.
> ![](https://cdn.hackclub.com/019e7a24-5e7b-79e6-81c8-b3ccb185c385/screenshot_2026-05-30_at_2.27.34___pm.png)
> Tada!!

## Adding Our Player Into The Game

Now drag the player file from the bottom left corner into your game just like so.

![](https://cdn.hackclub.com/019e7a2b-776a-79d4-8a3c-66d7563cc258/godot_2_.png)

Test the game out. Can you move the player with the arrow keys? Can you jump with the space button?

Now go into the player.gd script and change the const JUMP_VELOCITY  to equal 500.0. It should look like this:

```gdscript
const JUMP_VELOCITY = 500.0
```

## Making the Platforms

![](https://cdn.hackclub.com/019e7a35-3b89-7d0a-a7fb-2457d50a6abc/screenshot_2026-05-30_at_2.45.58___pm.png)

Name the `StaticBody2D` to be "Platform1" since the ground will technically be your first platform. Copy and paste that node and rename it to "Platform2" to make your second platform. Drag and resize it to where you want it to be.

![](https://cdn.hackclub.com/019e7a51-a15a-7009-8eee-1821dddfe15b/screenshot_2026-05-30_at_3.16.58___pm.png)

Place as many as you want, where you want them. Make sure to test your game to see if your character can actually jump on each platform!

## Adding in Garlics

Add in a `TextureRect` node. Rename it to "Garlic." Set its texture to a piece of garlic, or any image of your choice. Resize it and drag it to where you want your first piece of garlic to be. 

![](https://cdn.hackclub.com/019e7a65-194b-7e93-a62c-35fe39973717/screenshot_2026-05-30_at_3.38.14___pm.png)

Add an `AnimationPlayer` node. Rename it to be "animation." Add a `Node2D` node and add the `animation` and `Garlic` node to it. It should look like this: 

![](https://cdn.hackclub.com/019e7a6b-940e-7ff2-be4f-7ecbf30c6830/screenshot_2026-05-30_at_3.45.21___pm.png)

Now lets animate our garlic and give it some movement! Click the `animation` node and make a new animation at the bottom of your screen. Name it "floating," since we're making a floating effect.

![](https://cdn.hackclub.com/019e7a6f-be03-775a-ab27-03734410a7d6/screenshot_2026-05-30_at_3.49.42___pm.png)

Click on the `Garlic`. Go to the right side of the screen and click the key next to the Garlic's position. 

![](https://cdn.hackclub.com/019e7b68-7ed2-747f-be56-f536bd2b0e2f/26.png)

Drag the animation track to 1 second.

![](https://cdn.hackclub.com/019e7b68-8182-7801-bce9-5eba51a326eb/27.png)

Move the garlic a little bit up and click the key button again. Now your animation track should have two dots just as shown below.

![](https://cdn.hackclub.com/019e7b68-8480-74d0-873b-10b41853d8ef/28.png)

Set the animation to "Cubic" as shown below.

![](https://cdn.hackclub.com/019e7b68-87c9-7951-acbb-f7491131441c/29.png)

Double click the loop button in the animation track to make the animation loop!

![](https://cdn.hackclub.com/019e7b68-8a6b-7a57-b439-6b62b6d13bb0/30.png)

Now your simple animation is done! Now lets get started to adding in the garlic's hitbox. Add a `Area2D` node to the `Garlic` node. Add a `CollisionShape2D` node to the `Area2D` node. It should look like the image below:

![](https://cdn.hackclub.com/019e7b70-1f81-7cf6-ac94-9b88aa29db32/screenshot_2026-05-30_at_8.29.55___pm.png)

Move the `Area2D` to cover the garlic image. Resize it to completely cover it. 

![](https://cdn.hackclub.com/019e7b71-3116-7be3-85ad-0058aaa8f98c/screenshot_2026-05-30_at_8.31.07___pm.png)


Now, you can duplicate your Garlics all over your scene. Be sure to keep them in some kind of disorder to deter your player enough to create a challenge. 

> **Tip:** You can hit **Command+D** on your keyboard to duplicate nodes quickly.

# Programming the Platformer Minigame

For each garlic placed (just attach the same script to each by creating a script and dragging it from the menu under `Filter Scripts` to the chosen node):

```gdscript
extends Node2D
@onready var player: CharacterBody2D = $"../Player"
@onready var self_area = $Area2D
@onready var player_area = $"../Player/Area2D"

signal garlic_collected

func _ready() -> void:
	pass # Replace with function body.


func _process(delta: float) -> void:
	
	if player_area.overlaps_area(self_area):
		if self.visible:
			print_debug()
			emit_signal("garlic_collected")
			self.hide()
		
```
This is for the entire minigame, under the script for the entire scene: 
```gdscript
extends Node2D
@onready var themed_timer: Node2D = $ThemedTimer



var garlic_collected = 0
var timer_end = false

func _ready() -> void:
	await themed_timer.Timer(10.0)
	#after this is compeleted...
	timer_end = true

func _process(delta: float) -> void:
	
	if garlic_collected == 3:
		if Global.minigames_done > 3:
			get_tree().change_scene_to_file("res://scenes/done_screen.tscn")
		else:
			get_tree().change_scene_to_file("res://scenes/timer_screen.tscn")
	
	if timer_end:
		Global.minigames_done -=1
		Global.lives -= 1
		get_tree().change_scene_to_file("res://scenes/timer_screen.tscn")
		

func garlic_collect() -> void:
	garlic_collected = garlic_collected +1
	return

```

# Creating a Clicker Minigame
> To create the Clicker Game (the second minigame), starting is simple.

![Create a new scene](https://cdn.hackclub.com/019e7a09-646c-7ae0-a6ea-e03e7abd0c21/screenshot_2026-05-30_at_1.57.15___pm.png)

First, create a new scene by pressing the **+** at the top of the viewport. Create a new **2D Scene** and name it **Minigame_2**.

> **Note:** Name the scene exactly `Minigame_2`. Previously, in the timer screen code, we told Godot to load the next minigame by referencing a specific scene name. If the file is saved under a different name, the game won't be able to find it and everybody dies.

![Copy the background and platform](https://cdn.hackclub.com/019e7a0d-43d5-74c0-980f-c1436a64c0a7/screenshot_2026-05-29_at_9.46.34___pm.png)

Next, return to the first minigame and copy the **background**. Paste it into your new minigame scene to save time.

Now, we need our buttons. We want the player to tap all the buttons within a certain timeframe, and have a life removed if all 4 weren't pressed. To create a button, we can press the **+** in our Scene Tab, and look for a  **TextureButton**.

> **Tip:** You can hit **Command+A** on your keyboard to automatically add to the scene.

![ur gonna add a button, new texture to it, and rename the thingie](https://cdn.hackclub.com/019e7a4b-136e-787f-8eab-a4f01dbfcd86/screenshot_2026-05-30_at_3.07.08___pm.png)

You are going to add a garlic texture by traveling to the **Inspector** and dropping down the `Textures` tab. You should also rename your button `Button_1`, for cleanliness' sake.

Next, add a script to your Button. You don't have to do anything more, as we'll cover the programming in the next module. However, do know that the purpose of this script is to, first, detect a click and then hide the sprite so the player can focus on what's left. 

![](https://cdn.hackclub.com/019e7a5f-7062-78fa-86b6-022e14aaa4f3/screenshot_2026-05-30_at_3.20.12___pm.png)

Ignore the multiple Garlics here, we'll add them in our next module.

![](https://cdn.hackclub.com/019e7a5f-a5ce-7f36-90b7-aef921780d01/screenshot_2026-05-30_at_3.25.57___pm.png)

Now we need to focus on our timer. We want the buttons to all be pressed within 5-7 seconds, so we need a timer that detects if the time has ended or not.

Go to the **FileSystem** and select `themed_timer.tscn`. You want to drag it into the scene, wherever is most convenient. 


Now you're done setting your scene up. Time to program!!!!

![](https://media1.tenor.com/m/gFuIqmSvNRcAAAAd/rahhh.gif)

# Programming the Clicker Minigame

For this minigame, you need to remember we want the player to tap all the buttons within a certain timeframe, and have a life removed if all 4 weren't pressed.

The purpose of your button scripts is to, first, detect a click and then hide the sprite so the player can focus on what's left. 

To do that, enter this code into your button script:

```gdscript
extends TextureButton
@onready var parent = $".."

func _ready() -> void:
	pass # Replace with function body.

func _process(delta: float) -> void:
	pass

func _on_pressed() -> void: #YOU NEED TO CONNECT THIS SIGNAL FROM THE TAB NEXT TO INSPECTOR!!
	hide()
	parent.buttons_pressed += 1
```
And add this in your main scene's script, which you'll probably have to create:
```gdscript
extends Node2D
@onready var themed_timer: Node2D = $ThemedTimer

var buttons_pressed := 0
var timer_end = false

func _ready() -> void:
	await themed_timer.Timer(7.0)
	#after this is completed...
	timer_end = true 


func _process(delta: float) -> void:
	if buttons_pressed == 4:
		if Global.minigames_done > 3:
			get_tree().change_scene_to_file("res://scenes/done_screen.tscn")
		else:
			get_tree().change_scene_to_file("res://scenes/timer_screen.tscn")
	
	if timer_end:
		Global.lives -= 1
		Global.minigames_done -=1
		get_tree().change_scene_to_file("res://scenes/timer_screen.tscn")

```


Now, you can duplicate your Buttons all over your scene. Be sure to keep them in some kind of disorder to deter your player enough to create a challenge. Ignore the fact there's no script connected in the image, there should be scripts.

![I'm too lazy to write a description](https://cdn.hackclub.com/019e7a51-ecbf-7cfa-83d4-1022f9a45530/screenshot_2026-05-30_at_3.14.58___pm.png)

> **Tip:** You can hit **Command+D** on your keyboard to duplicate nodes quickly.

# Challenge: Creating the Winner and Death Screens

> CHALLENGE: This is your responsibility to make, and use what you've learned already to create a unique and personal one for your game. This will be judged by reviewers for originality.

![](https://media1.tenor.com/m/R1U76Ds4-kUAAAAC/peppa-pig-meme-peppa-pig.gif)

# Publishing and Submitting Your Game
> You're finally done with your project! Now, how do we get this project to be accessible online so you can share it to all your friends, family, or to other hackers? I gotchu.

First things first, go to the top of the screen and click "Project" and then "Export.."

![](https://cdn.hackclub.com/019e75d8-d9b6-7c0e-a324-532f45395f4d/19.png)

Add a preset called "Web." You may have to download it. After it's done, click "Export Project.." 

![](https://cdn.hackclub.com/019e75d4-4659-7333-9afd-11ba07969fd6/screenshot_2026-05-29_at_6.21.37___pm.png)

Create a folder called "exports" so we can keep track of all these files in one place. Name the file "index.html"

![](https://cdn.hackclub.com/019e75d8-dbf3-7100-90cc-1f61ac6922cd/20.png)

Click Save. Then find the exports folder in your file manager. 

![](https://cdn.hackclub.com/019e75d8-dde4-74a9-b819-40193ba7adeb/21.png)

Go inside and zip/compress all the files together. You can do this by holding shift and selecting all the files, and then right clicking to find a "zip" or "compress" option. 

![](https://cdn.hackclub.com/019e75d8-e011-7434-97e9-c327cfdbc2b7/22.png)

## Putting the Game onto Itch.io

Go to [itch.io](itch.io). Make an account. Go to the arrow on the left and click "Upload new project."

![](https://cdn.hackclub.com/019e75d8-e23a-7100-86b3-b3bee97757c3/23.png)


Make sure to:
1. Give the game a creative title
2. Make sure the Kind of Project is **HTML**
3. Upload the Archive.zip or the compressed file.
4. Make the game a Draft, and then make the game public after saving.

![](https://cdn.hackclub.com/019e7b91-c4ee-73ba-86a7-09b9705db506/6.png)
![](https://cdn.hackclub.com/019e7b91-8af6-7e0a-b23c-9ebc7bd8c7d0/7.png)

> Test your game on itch.io. Does it work? If something appears broken, go back through this section and see if you missed something.

Congrats on finishing your game! You're now like a Godot pro. 
![](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExbHh2ZjdwdmVwY2k3NmYyaXc1eXRhd2kwb2g2YjBhNjdjMGg2MDIzeCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/PgiMeF1tVKGVILW16h/giphy.gif)



