# Traffic Light System
## Overview
Traffic lights are signaling devices positioned at road intersections, pedestrian crossings, and other locations to control flows of traffic. An actual traffic light alternates the right way of road users by displaying lights of a standard color (red, yellow and green), using a universal color code.
The main objective of this traffic light controller is to provide sophisticated control and coordination to confirm that traffic moves as smoothly and safely as possible. This project makes use of LED lights and seven - segment for indication purpose and a microcontroller is used for auto changing of signal at specified range of time interval. LED lights gets automatically turns on and off by making corresponding port pin of the microcontroller “HIGH”.

## 7 SEGMENT DISPLAY: -
A seven-segment display is a form of electronic display device for displaying decimal numerals that is an alternative to the more complex dot matrix displays. Seven-segment displays are widely used in digital clocks, electronic meters, basic calculators, and other electronic devices that display numerical information.
There are two types of LED 7-segment displays: common cathode (CC) and common anode (CA). The difference between the two displays is the common cathode has all the cathodes of the 7-segments connected directly together and the common anode has all the anodes of the 7-segments connected.
## Working:
1. The main program at 0x0030H. Initially all ports are clear. Front signal is turned on. The program logic of getting quotient 1 is used.
2. The DATA is fetched from memory location 0x0300H and sent to PORT 2 to display on seven segment LED display. Similarly, for other values such as 9,8,7,6,5,4,3,2,1,0. The delay in microsecond is used between counts. The count happens for thirty-five times. When time is completed, Then Right Traffic signal is activated.
3. The Port P1 and P0 is activated. The light arrangement is reordered. The Program starts from X1 and Count again starts.
4. The 7 segment was used in this design to display the timing to the vehicle.
The process consists of five phases as listed:
#### PHASE I: North -
Initially, while north signal glows green for 10 seconds, the east signal would glow amber for 10 simultaneous seconds and all the south & west would glows red for 20 seconds simultaneously.
#### PHASE II: East -
Then, east signal glows green for 10 seconds, the south signal would glow amber for 10 simultaneous seconds, west glows red for 10 seconds and north glows red for 20 seconds.
#### PHASE III: South -
Then, south signal glows green for 10 seconds, the west signal would glow amber for 10 simultaneous seconds, north glows red for 10 seconds and east glows red for 20 seconds.
#### PHASE IV: West -
Then, west signal glows green for 10 seconds, the north signal would glow amber for 10 simultaneous seconds, east glows red for 10 seconds and south glows red for 30 seconds.
#### PHASE V: Pedestrian –
During the entire process mentioned above, it glow red at all the pedestrian signals (NESW). After the completion of one complete traffic signal cycle, all the pedestrian lights glows green for 30 seconds for the people to walk safely, while all the traffic signals in all directions glow red.

### simulation [images](https://drive.google.com/drive/folders/1Ww861JC95etuLu-qQsqSPUE1GqnWFCv2?usp=sharing)

## Conclusion
In this project we have implemented 4-way Traffic Light control system. This project is cost effective. Implementation of this project in present day will effectively solve the traffic congestion which is a severe problem in many modern cities all over the world.
Automatic Traffic control system is based on a very effective way of optimizing traffic, with redefinition of threshold values for a real time application. This works to control traffic on four-way roads according to traffic control barricades. This proposed system will be able to build a developed country with less traffic jams and it will also help the emergency vehicle to reach in time to the destination. So, this intelligent system will help us to control traffic in more autonomous way. Also this system would be helpful for the pedestrians who cross by, to walk pass safely.
