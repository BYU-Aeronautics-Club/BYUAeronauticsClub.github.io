---
permalink: /tutorials/manufacturing/lasercutter.md
title: "Using the Laser Cutter"
layout: single
sidebar:
    nav: "tutorials"
---

## Introduction

This document presents instructions for use of the laser cutter specifically with foam board planes. It is specifically for use with the CoralDRAW program and the Epilog M2 laser cutter, the software and machine available in the BYU Prototyping Lab. 

## Step 1 - Boot Up the Laser Cutter

The cutter takes a few minutes to initialize. Go ahead and flip the power switch to give it time to do so while you format your documents.

## Step 2 - Upload and Your Document

After opening CoralDRAW, go to File>>Open and select a PDF document you want to upload off the computer. It will prompt you to decide what to do with the text. Select the “convert to curves” option and what pages you want to import.

![alt text](_pages/figures/Coral_Text_1.JPG)

Normally, the program can’t match your text exactly and will propose a substitute font. Just use the default and accept. Your document is now uploaded and ready to format!

![alt text](_pages/figures/Coral_Text_2.JPG)

## Step 3 - Format Your Document

You want to get rid of any unwanted curves or lines before sending the job to the cutter. You can do this by selecting the pointer icon on the left-hand tool bar (see image below). There are lasso and square selection options. Click or encircle each thing you want to take off and press delete on your keyboard. You will also need to change the sheet size in the top left corner to match the area you are cutting. For standard foam board, we use 19.5” tall by 29.5” wide.

![alt text](_pages/figures/Pointer_Icon_3.jpg)

If you are having trouble fitting all your pieces onto one page, trying turning and rearranging. If you click on an object after selecting it, you can turn it. For the laser cutter to be able to print the lines you’ve made, they need to be “hairline” width (see image below). You can change the width by selecting all pieces and changing the width under the “Object Properties” bar on the right side. If it isn’t there, simply go to Window>>Dockers>>Object Properties. You may need to toggle a few things in there to get the width to show up.

![alt text](_pages/figures/Hairline_4.jpg)

## Step 4a - General Color Mapping

Now that your document is formatted, you need to tell the laser cutter what to do with the different colors. You can get color numbers by using the dropper on the left-hand toolbar. Go to color mapping by selecting File>>Print>>Properties. The window below will pop up. You will need to do a few things. First is to make sure the “Piece Size” matches the size you inputted before (29.5 horizontal and 19.5 vertical for foam board). Second, select “Vector” under job type. Raster will print using little dots and is very, very slow (only useful for cutting decorative pieces or photos). Third, set the power and speed to your desired defaults for this piece. For foam board, default should be 45 speed and 39 power. Frequency should almost never be changed.

![alt text](_pages/figures/Color_Map_Main_5.JPG)

## Step 4b - Specific Color Mapping

If you desire multiple cutting settings you will need multiple color mapping settings. Move to the “Color Mapping” tab. There are normally some default colors on there. You can get rid of them by pressing the minus button. To add a new color, use the color numbers you got from your document previously and input them and your desired speed and power for that color, then press the plus button. For most Flite Test planes, reds are half cuts at 75 speed and 15 power, and blues are surface scores at 92 speed and 6 power. Go ahead and press print, and your job will show up on the laser cutter!

![alt text](_pages/figures/Color_Map_Tab_6.JPG)

Tip 1: When using build plans from online sources, there are often multiple instances of the same color with slightly different color numbers. Watch out for these! If you don’t put them in your color mapping, the laser will just use your default setting!

Tip 2: On some FT plans, there are regions with a series of orange hash marks that are only meant to indicate that a certain region needs to be half-cut, etc. Instead of trying to remove all of these lines by hand, you can simply put in another mapped color that is at 100 speed and 0 power so that the cutter will simply move over them without cutting. 

Tip 3: If your cut is coming out the wrong size, check on the main printing window under one of the tabs to make sure it’s not set to “fit to page”. You want it set to “original document size”.


## Step 5a - Configuring the Laser Cutter Bed

Now that your document has been sent to the laser cutter, a few things need to be done to make sure it’s set up properly. To focus the laser cutter, first move the selection to “Focus” on the control panel on the right hand side using the selection arrows. Place your material on laser cutter in the back left corner and hang the focusing tool on the laser. 

![alt text](_pages/figures/Focus_Selection_7.jpg) ![alt text](.figures/Focus_Tool_8.jpg)

Then use the little knob to move the bed up until it just touches the material. Once it does, click the knob in so that it zeros the laser cutter. You should see a bunch of zeros on the little screen now when “Focus” is selected.

![alt text](_pages/figures/Focusing_9.jpg)

Next, select “Jog” using the arrows again and turn on the pointer light using the red laser button. This points to where the laser will cut your material. You want to move this to the very top left corner where your materials meets the measuring bars on the bed. Click the knob again to set that as your zero position. You are almost ready to cut!

## Step 5b - Checking Your Cut

We want to check that the job you sent to the cutter works properly. Move the selector to “Job” and select the job you want to cut out. **With the lid open** so it doesn’t cut, press GO. This will tell the cutter to start moving on the path for your cut. Having the lid open will keep the laser off so you can just follow the laser pointer and see where it’s cutting. You just want to make sure it is cutting in the area you told it to. Note that it is programmed to zig-zag all over instead of cutting one shape out at a time to avoid heating up any one area too much. Once you are satisfied, press STOP and RESET, close the lid, and press GO again. 

![alt text](_pages/figures/GO_10.jpg)

Tip: You can press STOP at any time to pause the cutter after it finishes its next cut vector. This is useful when there are two cuts close to each other that might cause overheating. Pressing RESET will start the job over while pressing GO will simply resume your cut.
