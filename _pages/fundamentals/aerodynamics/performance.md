---
permalink: /fundamentals/aerodynamics/performance/
title: "Performance"
layout: single
sidebar:
    nav: "fundamentals"

---

The way you design your UAV will be largely driven by the mission and design requirements you defined at the outset of your project. Depending on the mission, there are a large variety of aircraft that could be designed to fulfill your mission. However, there are some universal principles of flight that will be essential in determining the feasibility of your UAV. As you refine your design using these principles, your UAV will improve in its ability to perform as an aircraft and fulfill its mission.

## Aerodynamic Forces
All the forces we will discuss here can be directly attributed to either pressure or shear. A summary of these forces and how they produce lift and drag can be found in the section on [fluid mechanics](https://aeronautics.byu.edu/fundamentals/aerodynamics/fluids/). Here, we will focus more on calculating the magnitude and location of these forces and dealing with how they affect your aircraft. In general, you want to find ways to maximize lift while minimizing drag.

### Parasitic Drag
There are essentially three different types of drag that we are dealing with. Two of these (skin friction and pressure) can be summed up to become parasitic drag. Skin friction drag is caused by shear stress while pressure drag is caused by normal stress from pressure. Both of these will be factored into a single equation that can be used to calculate the total parasitic drag.

For skin friction, we want to calculate the *skin friction coefficient*, which is given the symbol C<sub>f</sub>. To calculate this completely accurately, it would be necessary to perform an integral of the shear stress across across the entire surface. Doing so is quite difficult, so we will use a simpler solution that is the analytical solution for a flat plate in laminar with no pressure gradient. This is called the Blasius solution and is summarized in the equation below.

![Cf Laminar](./figures/cf_laminar.JPG){: .align-center}

Since laminar flow only includes flow up to a Reynold's number up to 500,000, we can use the equation below for turbulent flow. 

![Cf Turbulent](./figures/cf_turbulent.JPG){: .align-center}

To factor in pressure drag, we will calculate a *form factor*, which is represented by a lowercase k. This accounts for the thickness of the surfaces that are producing lift. Since a typical small UAV travels at low speeds relative to the speed of sound, we can neglect compressibility factors and use the equation below where &#x03B3; is the [sweep](https://aeronautics.byu.edu/fundamentals/aerodynamics/configurations/#basic-geometry) angle of the surface and t/c is the [thickness-to-chord ratio](https://aeronautics.byu.edu/fundamentals/aerodynamics/airfoils/#naca-airfoils) of the airfoil.

![Form Factor 1](./figures/form_factor_wings.JPG){: .align-center}

For a body of revolution (such as a fuselage), we use a different formula based on on the *fineness ratio* (fr) which is defined as the length over the maximum diameter (l/d). For fineness ratios between 5 and 15, we can use the formula below to calculate the form factor. For fineness ratios over 15, the form factor will be 1. 

![Form Factor 2](./figures/form_factor_bodies.JPG){: .align-center}

Next we want to calculate the total area of the UAV that is exposed to air. This is typically referred to as the wetted area, or S<sub>wet</sub>. For a lifting surface, it can be approximated using the equation below. For a body of revolution, simply find the outer surface area of the shape.

![Wetted Area](./figures/swet_wings.JPG){: .align-center}

Putting this all together, we can calculate the parasitic drag for each component of an airplane using the formula below. To get the total drag, you will have add up the parasitic drag for each component individually since they have different form factors and wetted areas. 

![Parasitic Drag](./figures/parasitic_drag_formula.JPG){: .align-center}

To nondimensionalize this into a coefficient, we can use the definition of the drag coefficient and apply it to parasitic drag, as in the equation below. For this equation, S<sub>ref</sub> is simply the planform (or projected) area of the component. 

![Coefficient of parasitic drag](./figures/cdp_formula.JPG){: .align-center}

### Induced Drag

## Static Stability

## Dynamic Stability

## Measures of Performance
