---
permalink: /tutorials/prop/batteries/
title: "Batteries"
layout: single
sidebar:
    nav: "tutorials"
---
Many modern UAVs use electronic propulsion and control systems, as opposed to the older gas-propelled systems. Such a system requires power, namely in the form of a battery. The preferred battery type in the Aeronautics Club is the Lithium Polymer battery. This is due mainly to its relatively and high energy density and discharge capability. That being said, the main focus of this page will be on LiPo batteries, but care and use of other batteries will be covered.

## Battery Types
Although we primarily use LiPo batteries, there a few different battery types in popular use in the model aviation world. These include Lithium Polymer (LiPo), Nickel Metal Hydride (NiMH), Lithiu Iron (LiFe), and Lithium-ion (LI). There are various tradeoffs associated with selecting one battery over another including ease of use, energy density, capabilities, and lifespan. Cost and availability should also be considered. We will conduct a brief overview of each and their various characteristics.

### Lithium Polymer Batteries
LiPo batteries are by far the most widely used and available batteries in model aviation. This battery is highly stable and hard to mess up with. The energy is stored in a solid polymer electrolyte without the use of metallic nodes. Each battery has different sections called cells that provide a nominal voltage of 3.7V per cell. These cells can come in various shapes and sizes to provide various amounts of available energy. This energy is typically measured in milli-Amp-hours (mAh). The total size of the battery will depend on both number of cells and energy capacity. We will typically use 3s (3 cell) batteries to provide the desired voltage for our planes (11.1V), but it is typical to use 2-6s LiPo batteries based on the voltage you want.

Another important compontent of a LiPo battery is its discharge rate, or C rating. This is typically what distinguishes a lower-quality battery from higher quality ones. The C rating determines how much current can be drawn from the battery at any one time. For example, for a 20C battery with an energy capacity of 2000 mAh (or 2.0 Ah), the max discharge rate is 20x2.0 = 40 Amps. This should typically be about 15-20% above the max current draw of your propulsion system to avoid damaging the battery. LiPo batteries will typicall have much higher discharge rates than other battery types, including Lithium-Ion batteries (which have comparable energy density). 

When caring for LiPo batteries, it is important to maintain each cell within a certain voltage range. Chargers with LiPo battery charging capabilities will have a balance cable that allows the charger to charge each cell at the same rate, maintaining the same general voltage level. This is important in charging and discharge to preserve the stability of the battery. In general, each cell should also remain within a 3.6V-4.2V range. In any case, you should NEVER allow a cell to reach below 3.0V. Doing so will result in severe shortening of the cell's life cycle. When not in use, batteries should be stored at 3.7V per cell. This provides the longest lifespan. When LiPos reach the end of their life cycle or are misused, they tend to puff up. This is a tell-tale sign that you should consider disposing of them. This should be done using safety guidelines outlined by local laws and ordinances.

### Nickel Metal Hydride Batteries
Nickel Metal Hydride batteries are the worst.

### Lithium Iron Batteries

### Lithium-Ion Batteries

### Comparison Table

| Characteristic | LiPo | NiMH | LiFe | LI |
| ------- | -------- | --------- | --------- |
| Energy Density (Wh/kg) | 100-265 | 60-120 | 90-160 | 100-265 |
| Cycle Durability (#cycles) | 200-400 | 180-2000 | 2000 | 400-2000 |
| Average Price (Wh/dollar) | 2-4 | 1-3 | 3-4 | 3-4 |

## Charging LiPo Batteries
This section will step you through using the Turnigy chargers in the lab to charge LiPo batteries. Although you may be using a different type of battery, the general controls of the instrument will be the same.


### Step 1 - Power on DC Power Supply

![alt text](./figures/chargebatt1.jpg)

### Step 2 - Plug in Battery
For LiPo batteries, there are two leads that need to be connected to the charger so that the individual cells of the battery can maintain their balance. This particular battery is 3-cell (3S) and uses an XT-60 connector (pictured left) to plug into the charging port. Other connections will require different adapters. Plug the balance connector into the port with the same number of pins (pictured right).

![alt text](./figures/chargebatt2a.jpg) ![alt text](./figures/chargebatt2b.jpg)

### Step 3 - Initiate LiPo Program
When the charger turns on, the screen will most likely look like the picture below. If this is not the case, press the TYPE/STOP button a few times to back up to the PROGRAM SELECT menu (pictured right)

![bat3a](./figures/Bat3a.jpg) ![bat3b](./figures/Bat3b.jpg)

#### Step 3a - Enter Charging Menu
Once you get the LiPo BATT selection, press START/ENTER to enter the next level of menus. The screen will appear as below. You can cycle through different functions (charging, discharging, etc.) by pressing the STATUS buttons. We will be charging for this demonstration. When you get to CHARGE, press START.

![bat3c](./figures/Bat3c.jpg)

#### Step 3b - Adjusting Voltage and Ampage
Once in the CHARGE program, press START again to change the parameters for charging. You will typically set the current to the Ah rating of your battery, e.g. a 2200mAh battery should be set to 2.2A for charging. Press the STATUS arrow buttons to adjust the value. Press START again to move from current to voltage. For LiPo charging, there are fixed voltage values based on the number of cells (3.7V per cell). If there is not a clear indication of the number of cells, it is one less than the number of leads on your balance connecter. Press the STATUS arrow buttons to adjust this value, then press START one more time.

![bat3d](./figures/Bat3d.jpg)

#### Step 3c - Begin Charging
Once you have set the charging parameters, hold the START button until it checks battery status and the screen below and left appears. Check to make sure the numbers for R: and S: are the same then press START again and the screen below right will appear. The battery has now begun charging. You may press the STATUS arrow buttons to view the cell voltages, ending voltage, and several other things.

![bat3e](./figures/Bat3e.jpg) ![bat3f](./figures/Bat3e.jpg)

#### Step 3d - Finish Charging
The charger will stop charging automatically once it reaches the end voltage, but you may stop the charging process at any time by pressing STOP. It indicates the completion of the charging process with an on-screen message and a distinct jingling sound that will ring until you go to the charger and press STOP. You may now disconnect your charged battery for use!



### Step 4 - Turn off DC Power Supply

Do the right thing. Remember to turn it off.

![bat4](./figures/Bat4.jpg)





