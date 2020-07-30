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

<table>
    <thead>
        <tr>
            <td>
                <b>System</b>
            </td>
            <td>
                <b>Requirements</b>
            </td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                Aerodynamics
            </td>
            <td>
                <ul>
                    <li>Sufficient wing area to lift 1 kg</li>
                    <li>Fix-wing configuration</li>
                    <li>Conventional wing and tail</li>
                    <li>Static margin of 15%</li>
                    <li>Stable in all dynamic modes</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Structures
            </td>
            <td>
                <ul>
                    <li>Thick airfoil</li>
                    <li>6x6x6 cm candy cargo space</li>
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
                    <li>FPV camera system</li>
                    <li>6-channel Tx/Rx system</li>
                    <li>Ground-facing live video camera</li>
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
                    <li>10 min battery life at 50% throttle</li>
                    <li>3s LiPo battery (11.1V)</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

More requirements might be added further into the project, but this represents a good starting point for the candy drop. Notice that each system has specific, relevant requirements attached to them. 

### Key Performance Indicators
Some of these requirements are more qualitative, but many can be directly measured. To do so, you can create *key performance indicators* (KPI's) to measure your design against as it is being developed. This has been done for the candy drop in the table below. As you get more detailed in your design, you can add benchmarks (or goals) for each KPI as something to measure against.

<table>
    <thead>
        <tr>
            <td>
                <b>System</b>
            </td>
            <td>
                <b>KPI</b>
            </td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                Aerodynamics
            </td>
            <td>
                <ul>
                    <li>Wing area (m<sup>2</sup>)</li>
                    <li>Static margin (%)</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Structures
            </td>
            <td>
                <ul>
                    <li>Airfoil thickness (mm)</li>
                    <li>Cargo space volume (cm<sup>2</sup>)</li>
                    <li>CG position change after drop (mm)</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Controls
            </td>
            <td>
                <ul>
                    <li>Number of Tx/Rx system channels</li>
                    <li>Tx/Rx system frequency (GHz)</li>
                    <li>FPV system range (km)</li>
                    <li>FPV system frequency (GHz)</li>
                    <li>Camera resolution (megapixels)</li>
                </ul> 
            </td>
        </tr>
        <tr>
            <td>
                Propulsion
            </td>
            <td>
                <ul>
                    <li>Motor power rating (kV)</li>
                    <li>Propeller diameter (in)</li>
                    <li>Battery voltage (V)</li>
                    <li>Battery energy storage (mAh)</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
