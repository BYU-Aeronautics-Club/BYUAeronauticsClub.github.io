---
permalink: /fundamentals/designtools/testing
title: "Testing"
layout: single
sidebar:
    nav: "fundamentals"
    
---

One of the most critical parts of your design project is the testing you will be conducting to ensure it is airworthy and performing as expected. This is done through a number of tests both on the ground and in the air. You will want to test components, aerodynamics, propulsion, and the complete UAV. It is important to have an objective in mind with any test you conduct so the results can inform any design changes you might need to make. When done in tandem with [prototyping](https://aeronautics.byu.edu/fundamentals/designtools/prototyping/), testing can be an immensely useful tool during your design project.

## System Testing
As mentioned in the section on [mission requirements](https://aeronautics.byu.edu/fundamentals/designtools/definingrequirements), your UAV can be broken down into several different systems (commonly the airframe, structure, controls, propulsion, and payload). Each of these systems should be tested separately to ensure they meet the proper requirements before assembling and advancing your design. Below is a list of possible components you could test for various systems:

+ Motor and propellor
+ Transmitter connectivity
+ Airframe stress
+ Component adhesion
+ System modularity
+ Autonomous flight system
+ Electronics configuration
+ Landing gear
+ Rx/Tx range
+ Battery

## Glider Testing
Pretty much as quickly as possible, you ought to begin working on a simple prototype in order to test the airframe design. This can be done intially with cheap and workable materials such as a [foam wing](https://aeronautics.byu.edu/tutorials/foamcutter/) and a body made from DTFB. Other similar materials may be more desirable for your project. When constructing your prototype, you should be careful to match the CG location to where is in your design. The idea is to get a to-scale prototype of your UAV that is as close as possible to your design to test its airworthiness. 

When you are flying the glider, there will be no propulsion system onboard. This means your are merely testing its aerodynamic characteristics. This should be done on a good-sized hill so you can observe the behavior of the glider over an extended period before it lands. One thing this should tell you is the [lift to drag ratio](https://aeronautics.byu.edu/fundamentals/aerodynamics/performance/#lift-to-drag-ratio), which is a good indicator of good design if in the proper range. You should also be looking for [stability behavior](https://aeronautics.byu.edu/fundamentals/aerodynamics/performance/#static-stability), such as being tail-heavy or nose-heavy. The glider should not turn too much on its own either. You are looking for a long, steady glide with little difficulty. 

Note: Windy conditions may make it difficult to reliably test your glider, especially if it is very light.

## Wind Tunnel Testing
In order to verify your aerodynamic design calculations, you may want to conduct some wind tunnel testing. This can be done with a prototype of the same variety used for glider testing. Although there are numerous applications for the information this test would reveal, the basic data produced will always be the same; lift, drag, and angle of attack. You should be careful to make sure your calculations used for design match up well with the test results.

Since the testing equipment only measures forces, a scale model of the plane will produce measurements that are not comparable to your full-size calculations. To remedy this, you should instead calculate the coefficients and compare those. If your calculations are perfect, they should be identical to your test results.

If you wish to use the wind tunnel at BYU, you must speak with the ME facilities manager, Kevin, to make arrangements. You will likely not get permission to use it unless you are part of the competition team.

## Flight Testing
Once you have completed and assembled your design, you will want to perform flight tests to see if all of your hard work has paid off! Before doing so, it is essential that you create a *pre-flight checklist*. This is essentially a list of items to be performed before takeoff to make sure all systems are connected properly and all safety requirements are being met. Below is an a checklist used previously by the Boeing AerosPACE capstone team.

<table>
    <thead>
        <tr>
            <td>
                <b>System</b>
            </td>
            <td>
                <b>Action Item</b>
            </td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                Battery
            </td>
            <td>
                <ul>
                    <li>Charged</li>
                    <li>Secured in Plane</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Connections
            </td>
            <td>
                <ul>
                    <li>Connections Secured</li>
                    <li>Components Secure</li>
                    <li>Wire Integrity</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Propulsion
            </td>
            <td>
                <ul>
                    <li>Proper motor direction</li>
                    <li>Propellor securedm</li>
                    <li>Propellor balanced</li>             
                </ul> 
            </td>
        </tr>
        <tr>
            <td>
                Cameras/FPV
            </td>
            <td>
                <ul>
                    <li>Established camera output</li>
                    <li>Ground station receiving</li>
                    <li>OSD visible</li>
                    <li>Camera switching functioning</li>
                    <li>VTX frequency</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Servos
            </td>
            <td>
                <ul>
                    <li>Control linkage integrity</li>
                    <li>Hinges function properly</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Wing Mount
            </td>
            <td>
                <ul>
                    <li>Wind secured to mount</li>
                    <li>Mount secured to body</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Motor Mount
            </td>
            <td>
                <ul>
                    <li>Secured to plane</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Tail
            </td>
            <td>
                <ul>
                    <li>Secured in upright position</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Fuselage
            </td>
            <td>
                <ul>
                    <li>All components secured</li>
                    <li>No rips or tears</li>
                    <li>Adhesives holding</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Takeoff Weight
            </td>
            <td>
                <ul>
                    <li>Matches expected value</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Autopilot/iNav
            </td>
            <td>
                <ul>
                    <li>Wire connections</li>
                    <li>Servos react</li>
                    <li>GPS lock</li>
                    <li>Proper mission saved</li>
                    <li>Altitude below 400 ft</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Transmitter
            </td>
            <td>
                <ul>
                    <li>Manual control of actuators</li>
                    <li>Switches in default positions</li>
                    <li>Charded</li>
                    <li>Control surface direction</li>
                    <li>Ensure mode switch works</li>
                    <li>Failsafe activates properly</li>
                    <li>Arm check</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>
                Weather
            </td>
            <td>
                <ul>
                    <li>Precipitation</li>
                    <li>Wind direction and speed</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

As you can see, the list is quite extensive. It covers anything you might forget to check that could cause any sort of mission or system failure. If your UAV fails in flight, you might make similar system checks after recovering it. 

Once the checks have been made, you should test your UAV's ability to fulfill various mission components. This can be done in pieces or all once, depending on your mission's complexity. If sub-systems can be checked in-flight, do so to ensure there are no issues when power is being drawn to the propulsion and aerodynamic systems. And don't forget to have fun!
