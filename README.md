# Laptop-Charger

**Problem statement:**

Design a circuit of Laptop Charger which will take input of 13V DC and gives output of 19V DC.

**MATERIALS USED:**
* LM3254
* 4.4k ohm Resistor
* 2.4k ohm Resistor
* 12k ohm Resistor
* 0.04 ohm Resistor
* 2.7 ohm Resistor
* 2.2k ohm Resistor
* 1M ohm Resistor
* 1k ohm Resistor
* 470 ohm Resistor
* 1.8k ohm Resistor
* 20V, 1000µF Capacitors
* 20V, 10µF Capacitors
* 0.1µF Capacitors
* 0.022µF Capacitors
* 1000pF Capacitors
* 25V, 4.7µF Capacitors
* 1N4148 Diode
* SB580 Diode
* BC547 Transistor
* BUZ78 Transistor
* Connectors
* 100µH Inductor
* 10A Fuse
* Connecting wires
* Power supply
* General Purpose Board
* Copper Clad


he schematic and footprint allocation for our circuit is as below:

KiCAD Schematic:

![Schematic](https://user-images.githubusercontent.com/42312238/80627431-82474a80-8a6d-11ea-82be-64cf8c8359ea.PNG)


Footprint Allocation to the Schematic:

![footprint 1](https://user-images.githubusercontent.com/42312238/80627454-8f643980-8a6d-11ea-8b1f-aabb89a61953.PNG)
![footprint 2](https://user-images.githubusercontent.com/42312238/80627464-91c69380-8a6d-11ea-9d92-40d7d5ae44c2.PNG)


**KiCAD GERBER FILE GENERATION:**

After footprint allocation, we move to net-list generation which is the process of importing the footprint allocation onto a virtual PCB. Here, we can place the components in the most effective manner onto our PCB board and can hence visualise how our final PCB structure look like by viewing the virtual 3D model. We can then complete the tracking and override them to make it most effective. We can choose the layers of the PCB we need in our final output and create a gerber file of it. We can save the gerber file in PDF format also. This PDF file is collection of all the layers of the PCB that we choose to have. Out of all of these files, the most important one is B.Cu file. It is the back copper tracking between all these components of our final PCB.

Final PCB Layout:

![PCB design 1](https://user-images.githubusercontent.com/42312238/80627507-ac990800-8a6d-11ea-853a-860cb7f0888f.PNG)
![Final PCB design](https://user-images.githubusercontent.com/42312238/80627521-b3c01600-8a6d-11ea-840d-dcbce8eb47cc.PNG)



The 3-D view of front-side and back-side our PCB is as below:

![Final PCB F](https://user-images.githubusercontent.com/42312238/80627569-cb979a00-8a6d-11ea-8237-9f15f2bda575.PNG)
![Final PCB B](https://user-images.githubusercontent.com/42312238/80627574-cdf9f400-8a6d-11ea-96ef-0c2830998f30.PNG)



**TONER TRANSFER:**

Toner transfer is the process by which we create our actual track of our circuit. We take the B.Cu file (PDF Format) and get it printed on a photo paper with a good quality ink. After the printout is taken, it is placed upside down on the copper clad and is taped down to it. We then cover it with a piece of cloth and heat it with the help of Iron. We press it down and run the iron over it until the ink is transferred onto the copper clad from the paper. This process of transferring ink from photo paper onto copper clad is called toner transfer.


**ETCHING:**

Etching is a method used for the production of the PCBs where acid is used to remove unwanted copper from a prefabricated laminate. This is done by applying a temporary mask (in our case, ink), that protects part of the laminate from the acid and leaves the desired copper layer untouched. The etching solution used by us is ferric chloride. Thus, we dip the PCB in boiling FeCl3 solution and wait until the excess copper is dissolved off and only our tracks of circuit remains. After this is done, we take out the board and clean it using water.


**DRILLING AND SOLDERING:**

After cleaning the board, we proceed to drill the board using a PCB drilling machine. We make holes of diameter approximately 1mm. Holes are made wherever components have to be placed. After all the holes are drilled, we proceed to place the components in their respective slots following the PCB layout. Once the components are placed, we solder them so that they stay in place and the connections are complete. We also solder other wires where external connections are required. After soldering, we clean our PCB with IP(Iso-propyl Alcohol) so that the residue of solder is removed. Now our circuit is ready to use. 

Now, we provide the trigger pulse to the input terminal of our circuit and check the operation of the buzzer. If all the above process are carried out in the correct manner, then our buzzer should buzz with the appropriate time intervals.


Actual PCB *(Circuit on General Purpose Board)*:

![GPB Front](https://user-images.githubusercontent.com/42312238/80627705-f08c0d00-8a6d-11ea-8d85-63758787bc2f.jpg)
![GPB Back](https://user-images.githubusercontent.com/42312238/80627735-fb46a200-8a6d-11ea-86e9-51a0add722bc.jpg)


Actual PCB *(Circuit on Copper Clad)*:

![PCB Front](https://user-images.githubusercontent.com/42312238/80627810-144f5300-8a6e-11ea-8937-53f7f8a9757d.jpg)
![PCB Back](https://user-images.githubusercontent.com/42312238/80627816-16b1ad00-8a6e-11ea-9749-55d99d9c78ba.jpg)
