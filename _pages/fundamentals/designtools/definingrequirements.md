---
permalink: /fundamentals/designtools/definingrequirements
title: "Defining Requirements"
layout: single
sidebar:
    nav: "fundamentals"
    
---

Whether or not you know it, the UAV you are planning to build right now has a specific mission it needs to fulfill. For many beginners, this can be as simple as having the capability to take off, fly for 5 minutes, and then land. Perhaps you want to lift a payload or achieve a certain speed. In any case, it is essential to be able to determine the *mission requirements* of your specific UAV project before even thinking about design. Doing so properly will serve to drive your project from start to finish.

## Mission Requirements
Before defining what your mission requirements are, you will need to first think about what is you want your UAV to do. This should be very specific. As an example, we'll say you want to build a UAV that can carry a small package of candy to your friend that lives two blocks away with a limited budget. You might define the following as your mission requirements:

+ Payload capacity of 100g
+ 10 minute flight time
+ Capable of flying without line of sight (LOS)
+ Capable of dropping payload remotely and accurately
+ Fixed-wing configuration
+ Hand launchable
+ Costs under $100 to make

These mission requirements would then become your main considerations for most any design decision you make.

### Concept of Operations
One way of visualizing your mission is to create a Concept of Operations, or Con Ops. This will lay out the different stages of your mission that need to be fulfilled using a a simple diagram or flow chart (see Figure 1). It can help you to have a better picture of everything that is required. This is turn will minimize the chances of neglecting any important mission requirements.

{% include figure image_path="_pages/fundamentals/designtools/figures/conops.JPG" caption="Figure 1: Example of a Concept of Operations for a simple mission." %}

## System Requirements
Once you have an idea of what your mission requirements are, you can start translating them into specific requirements for each of the systems in you UAV. You might categorize your systems as follows:

+ Aerodynamics
+ Structurers
+ Controls
+ Propulsion

Each of these systems has a different function within the UAV, and will therefore be tied to different requirements. System requirements are generally much more specific than mission requirements, and typically much more measurable. You might even need to do some basic calculations to find good metrics to compare to. Continuing with our "candy drop" example, we produce the table of requirements below.

<style type="text/css">
    table th {background-color:gray; color:white;}
</style>

<table>
    <tbody>
        <tr>
            <th>System</th>
            <th>Requirements</th>
        </tr>
        <tr>
            <td>
                Aerodynamics
            </td>
            <td>
                <ul>
                    <li>Sufficient wing area to lift 1 kg</li>
                    <li>Fix-wing configuration</li>
                    <li>Conventional wing and tail</li>
                    <li>High dynamica nd static stability</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Structures
            </td>
            <td>
                <ul>
                    <li>1"x1"x1" candy cargo space</li>
                    <li>CG position maintained after drop</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Controls
            </td>
            <td>
                <ul>
                    <li>Remote activated bomb bay</li>
                    <li>FPV system when not in LOS</li>
                    <li>6-channel communication system</li><li>Ground-facing camera</li>
                </ul> 
            </td>
        </tr>
        <tr>
            <td>
                Propulsion
            </td>
            <td>
                <ul>
                    <li>Sufficient thrust for hand launch</li>
                    <li>10 min battery life at 50% throttle 3s LiPo battery</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

Notice that //FIX ME

### Key Performance Indicators
