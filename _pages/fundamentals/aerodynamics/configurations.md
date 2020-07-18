---
permalink: /fundamentals/aerodynamics/configurations/
title: "Configurations"
layout: single
sidebar:
    nav: "fundamentals"

---

As a general class of aircraft, a UAV can be just about any flying vehicle that does not contain a person. In the Aeronautics Club, we deal primarily with fixed-wing UAV's, which generate lift through aerodynamic forces using the shape of the aircraft itself. Although you may be most comfortable with the conventional aircraft design, there are many fixed-wing configurations worth exploring that can produce desirable characteristics. Selections should be made based on your mission and performance requirements. Here we present a non-exhaustive list of some alternatives for wing, engine, and tail designs.

## Aircraft Geometry

## Wings
### Conventional
The conventional wing configuration features a single, forward wing paired with a tail toward the back of the UAV. Since the wing generates most of the lift, it creates a slight moment around the center of gravity (CG). The tail is placed at the back of the UAV to offset the aerodynamic moment from the wing, making it statically stable. A conventional wing is very stable and easy to work with. This is a good choice when a project has limited design time or expertise are limited. It is by far the most commonly used configuration, and for good reason. There is some lack of flexibility if you have a unique mission requirement that needs some additional creativity in design, or want to pursue a more interesting design path.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/conventional_wing.JPG" caption="Figure 1: Conventional wing" %}

### Flying Wing
Another common configuration for small UAV's is the flying wing. Unlike other common designs, the flying wing has no tail. The stability is instead provided by a highly swept wing, typically with vertial stabilizers on the ends. Popular examples of this are the [B-2 Stealth Bomber](https://en.wikipedia.org/wiki/Northrop_Grumman_B-2_Spirit "B-2 Bomber") and the updated [B-21 Raider](https://en.wikipedia.org/wiki/Northrop_Grumman_B-21_Raider "B-21 Raider"). One of the main advantages of the flying wing is the high acrobatic ability and maneuvarability. This can be attributed to its lower stability due to the lack of tail. The lowered stability makes it difficult to control, especially for a new pilot without a lot of flying experience. Although difficult to design, it can be a lot of fun to fly.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/flying_wing.JPG" caption="Figure 2: Flying wing" %}

### Biplane
The biplane configuration, although not very common, has the advantage of providing large amounts of lift with a relatively small span. This can be advantageous for a project where a smaller span is a design requirement. The tradeoff, however, is decreased aerodynamic efficiency. This is largely due to the interaction between the two wing surfaces. The lower wing receives downwash from the upper wing, infringing its ability to generate lift. In addition, splitting the wing into two pieces will increase the surface area needed to create the same amount of lift, greatly increasing the drag on the UAV.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/biplane_wing.JPG" caption="Figure 3: Biplane wing" %}

### Canard
Some flexibility in the longitudinal positioning of the wing is offered in the canard configuration. It features a wing placed at the rear of the UAV with a horizontal stabilizer at the front. This is common on business-class jets such as the [Piaggio P180](https://en.wikipedia.org/wiki/Piaggio_P.180_Avanti "Piaggio P180") because it allows the engines to be mounted in the rear to reduce noise in the cabin. Since the wing is far aft of the center of gravity, the horizontal stabilizer is placed in front to provide static stability. This could be useful in a situation where greater access to the fuselage is needed or rear motor placement is necessary. The drawback is the increased complexity in the aerodynamic design that would likely result in a less stable configuration for a small UAV.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/canard_wing.JPG" caption="Figure 4: Canard wing" %}

### Tandem
The last wing configuration we will mention is the tandem, which merely replaces the tail with a second wing. Much like the biplane, this allows for a UAV that has a much shorter span that produces the same amount of lift. Also like the biplane, the aft wing will receive downwash from the front wing, reducing aerodynamic efficiency. Some common applications in industry are small, personal aircraft and long distance flyers. 

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/tandem_wing.JPG" caption="Figure 5: Tandem wing" %}


## Tails
### Conventional
The conventional tail design for a UAV consists of a single vertical stabilizer intersected by a single horizontal stabilizer. The horizontal stabilizer is placed at the bottom of the tail. This is a tried and true tail design that is simple, stable, and easy to design. The first successful jumbo-jet commercial airliner, the [Boeing 747](https://en.wikipedia.org/wiki/Boeing_747 "Boeing 747") is a prime example of this. The main disadvantage is the downwash it receives from main wing since they are on the same plane (no pun intended). However, this positioning also gives the pilot greater control with the elevator near stall.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/conventional_tail.JPG" caption="Figure 9: Conventional tail" %}

### T-Tail
The t-tail is essentially just a modified conventional tail. The only difference is the horizontal stabilizer is placed at the top of the tail instead of the bottom. This prevents it from receiving downwash from the main wing in level flight, increasing aerodynamic efficiency. One problem this creates is that at high angles of attack, the horizontal stabilizer can be completely enveloped in turbulent air from the main wing, making it difficult to recover from stall. In addition, the higher placement necessitates a stronger vertical stabilizer.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/t_tail.JPG" caption="Figure 10: T-tail" %}

### V-Tail
Although not as common as the first two tails mentioned, the v-tail remains a popular selection for small UAV's. Instead of a vertical and horizontal component, the tail features two stabilizers at equal angles (usually 45° from horizontal). Some channel mixing or specialized electronics are required for this type of tail to function with a standard transmitter since yaw and pitch have been coupled. This can be more complex to design effectively, and typically results in some adverse moments occurring at the tail. At the same time, there is less surface interaction between the two components, increasing aerodynamic efficiency. The angle also means hardly any downwash is being received from the main wing.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/v_tail.JPG" caption="Figure 11: V-tail" %}

### H-Tail
The h-tail is a unique design that uses two vertical stabilizers instead of one. They are typicall placed at the far ends of the horizontal stabilizer, creating the shape for which the design is named. The twin surfaces allow for a much shorter and stronger tail with greater yaw control. The vertical stabilizer manufacturing and placement must be done very accurately to avoid deficiencies. This is difficult to do when working with foam or a similar material.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/h_tail.JPG" caption="Figure 12: H-tail" %}

## Engines
### Tractor
The majority of small UAV's operate with a single, front-mounted engine to provide thrust. The engine pulls the UAV along and is called a "tractor" motor. Much like front-wheel drive on a car, this configuration is generally more laterally stable than a UAV being "pushed". With the engine mounted on the front, it receives "clean" that hasn't been mixed around by the aircraft yet. This increases motor efficiency, which is typically below about 40%. The motor on the front also makes it easier to avoid getting clipped by the propeller when launching by hand. If fuselage is large in diameter compared to the motor, this will greatly increase its effectiveness. If this is the case for your UAV, looking into other mounting options is highly recommended.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/puller_motor.JPG" caption="Figure 6: Tractor motor" %}

### Pusher
If the motor is mounted facing backward on the UAV, it is simply called a "pusher". This is common on flying wing configurations to increasing the wing's effectiveness since it's the only lifting surface. The downside is that instead the motor is receiving downwash from the wing, decreaseing its efficiency. To prevent this problem, it is common to use a pod potruding from the top of the UAV to mount the motor. This way there is very little aerodynamic interaction between the motor and lifting surfaces and greatly decreased risk of propeller damage during landing. The addition of the pod will, however, also increase drag on the UAV.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/tractor_motor.JPG" caption="Figure 7: Pusher motor" %}

### Twin Motor
For small UAV's it normally makes more sense to use just one motor. For the most part, they are not large enough to merit a second motor. If you do choose to use a twin motor configuration, there are several advantages. Twin motors are typically mounted under (or on top of) the wings so they are far enough apart not to interact. One motor should turn counterclockwise while the other turns clockwise. This allows the roll and other adverse moments from the propellers to essentially cancel each other out, increasing stability. Like the pusher motor, this also increases motor efficiency since they are not in front of the fuselage. Having two engines also provides some redundancy should one engine fail during flight. You can usually get two small engines much cheaper than a single large engine for the same power. The tradeoff is that the total engine weight and power consumption for the same power will be noticeably greater. Great care should be taken to properly design and mount your propulsion system so it is not unbalanced.

{% include figure image_path="_pages/fundamentals/aerodynamics/figures/twin_motor.JPG" caption="Figure 8: Twin motor" %}

