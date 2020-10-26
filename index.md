---
layout: default
---

_“Spark AR for teens (Hour of code edition)  - tutorial for kids 11+ designed for [Hour of code initiative](http://code.org/learn) to create the first ever filter and introduce AR technology”_

### Why?

We want to help teens (11-19 years old person) discover other, technical side of Instagram and show huge field to express creativity, show what they care about. 

### How?

We are creating end-to-end tutorial for getting start with Spark AR - and after that they can easily use official Spark AR tutorial.


### Who?

Our key target audiences are:

* Software developers who want to use this guide and templates to create remarcable hour of code with AR effects.  
* Teachers - to add innovatative AR technology to their lesons



### Spark AR for 	Teens (Hour of code edition)  
 
### Introduction 
You for sure at least one time in your life used Instagram or SnapChat mask, or tried to catch Pokemons - and all this staff is based on Augmented reality technology. 

**Augmented reality** (often known as AR) is a computer technology that shows digital images on top of the current real world. For example it can show a digital table on top of a floor. It is different from virtual reality which makes a person feel they are somewhere else.  
Mostly, you are using Instagram mask for fun - but AR technology can be used for: 
- develop creativity 
- education purpose (history, science etc) 
- AR masks are often uses for Ads 
AR developer is a real job, where you can apply your STEM knowledge and express your creativity. 
So from now, if your parents said that you waste time on social media - you can answer that you are doing recherch for your future well-paid job. 

And today we will create your first Instagram filter - so let's start building! 
This tutorial is for absolute beginner 
This tutorial is created for version Spark AR Studio v99. 
 

### Getting Started

Installing Spark AR Studio  is fairly straightforward - but it should be done at least one day before 
(file around 400Mb) 
Here is direct link for loading:

- [Spark AR Studio for Windows](https://www.facebook.com/sparkarwindows/download)
- [Spark AR Studio for macOS](https://www.facebook.com/sparkarmacos/download) 
- or use from official site [https://sparkar.facebook.com/](https://sparkar.facebook.com/ar-studio/learn/downloads/)

<img src="{{site.url}}/images/image1.png" style="display: block; margin: auto;" /> 

***Hair Segmentation***


In this tutorial you’ll use the standard material and a light to create a hair segmentation effect. You’ll also add interactivity, to change hair color when the screen is tapped.

Hair segmentation is achieved with a hair segmentation mask texture, which you can create in Spark AR Studio. You’ll combine this texture with the camera texture in a material, then experiment with settings in the material to apply all kinds of visual effects to the hair.

Download the sample content to see the finished effect.

Creating the textures
Let’s take a quick look at how these textures work together to achieve hair segmentation:

The camera texture represents the live video captured by the camera when an effect is being played. When combined with a material, you can adjust the properties in the material to change the pixels in the camera texture - for example changing the color in a filter effect.
The hair segmentation texture separates a person’s hair from the rest of the scene.
Combining these two textures in the same material lets you to change the color of the hair, by manipulating the pixels in this part of the camera texture only.

The hair segmentation texture

To add the hair segmentation texture to your project:

In the Scene panel, select Camera.
Go to the Inspector.
Next to Segmentation, click +.
Select Hair.


A texture called hairSegmentationMaskTexture0 will be listed in the Assets panel.

The camera texture

Now add the camera texture:

In the Scene panel, select Camera.
In the Inspector, go to Texture Extraction.
Next to Texture Extraction, click +.
A texture named cameraTexture0 will be listed in the Assets panel:



Adding a rectangle
A rectangle will render the textures and material in the scene.

To add the rectangle:

Click Add Object.
Select Rectangle - it’ll automatically be added to the scene as a child of a canvas:


The rectangle should completely cover the device’s screen. To do this, adjust the rectangle’s properties:

Go to the Inspector.
Change the Size properties to Fill Width and Fill Height.


Creating a material
To create the material you’ll add the textures to:

Select rectangle0 in the Scene panel.
In the Inspector, go to Create New Material and click +.
A new material will be added to the Assets panel. Rename it hair_mat.



Editing the material.

Add the textures you’ve already created to the material:

Go to the Inspector.
Under Diffuse, click the dropdown next to Texture and select cameraTexture0.
Check the box next to Alpha.
Next to Texture, click the dropdown and select hairSegmentationMaskTexture0.
You’ll see the video of the camera texture playing in the Simulator:



Changing the hair color

To give the hair a different color:

Select hair_mat in the Assets panel.
In the Inspector, go to Diffuse.
Next to Color, click the rectangle and choose a color.


It’s worth experimenting with the opacity of the material, for a stronger or more subtle effect. To do this, adjust the slider next to Opacity in the Inspector.



For this tutorial set Opacity to 80%.

Editing the Render Options

Editing the Render Options in the material will change appearance of the hair color, so it’s worth experimenting with these settings. For this tutorial:

Change Blend Mode to Add.




***Don't forget to save your project:***

- Click File in the navigation bar and then select either Save or Save As...
- Enter a title, location and tags, if required
- Click Save 
Spark AR will create folder with title which you have given, and file *.arproj extention inside. 

To open your previous mask - just click on file *.arproj extention or if you work in Spark AR follow File > Open from main menu on top. 

***To try on your effect:*** 
On left menu find button "Test on device" (in red rectangle) > click "Send to App" > click "Send" near instagram camera (wait a moment for message "We've sent a notification ..." ) > Copy link  

<img src="{{site.url}}/images/image2.png" style="display: block; margin: auto;" /> 

Open this link on a mobile device to see the effect

***Congratulations!***
🎉🎊 ***You created your first Instagram effect!***  🎊🎉 

 
Now you  can surprise your friends by just sharing your preview link.

If you want you can publish your Instagram effect - follow this [instruction](https://sparkar.facebook.com/ar-studio/learn/publishing/publishing-your-spark-ar-effect/)  but it will take some time (up to 10 days)  




