# WATER LEVEL INDICATOR 

 - The Water Level Indicator employs a simple mechanism to detect and indicate the water level in  an overhead tank or any other water container.
 - The sensing is done by using a set of nine probes which are placed at nine different levels on the tank walls (with probe 9 to probe 1 placed in increasing order of height, common probe (i.e. a supply carrying probe) is placed at the base of the tank).
 - The level 8 represents the “tank full” condition while level 0 represents the “tank empty” condition.

 - In this project we show the water level indicator using eight transistors which conducts as level rises, a buzzer is also added which will automatically start as the water level becomes full, auto buzzer start with the help of microcontroller. With the help of this project we not only show the level of water on seven segment display but also indicate the water full condition using a buzzer.


 - When the water-level is below the minimum detectable level (MDL), the seven segment display is arranged to show the digit 0, indicating that the tank is empty, when the water reaches level1 (but is below level2) the connection between the probes gets completed (through the conducting medium – water) and the base voltage of transistor increases.

 - This causes the base-emitter junction of transistor to get forward biased, this switches transistor from cut-off to conduction mode thus PIN (B7) of microcontroller is pulled to ground hence, the corresponding digit displayed by the seven segment display is 1.

 - The similar mechanism applies to the detection of all the other levels. When the tank is full, all input pins of microcontroller become low. This causes the display to show 8 and also in this case a buzzer sound is given, thereby indicating a “tank full” condition.

 - Most water level indicators are equipped to indicate and detect only a single level. The Water Level Indicator implemented here can indicate up to nine such levels and the microcontroller displays the level number on a seven segment display.

 - So, the circuit not only capable of cautioning a person that the water tank has been filled up to certain level, but also indicates that the water level has fallen below the minimum detectable level. This circuit is important in appliances such as the water cooler where there is a danger of motor-burnout when there is no water in the radiator used up also it can be used in fuel level indication.



=======
## Block Diagram :-
![Blockdiagram](https://user-images.githubusercontent.com/98821876/155511413-d8af4434-e87a-4393-be53-94ac591fc427.png)
=======


## Components Required :- 

 - ATMEGA8 :- 
         - The ATmega8 is a low-power CMOS 8-bit microcontroller based on the AVR RISC  architecture. By executing powerful instructions in a single clock cycle, the ATmega8 achieves throughputs approaching 1 MIPS per MHz, allowing the system designer to optimize power consumption ver- sus processing speed.
         - There are 3-Internal Timers are accessible, 8 bit-2, 16 bit-1, presenting numerous operating modes & supporting internal/external clocking. Serial Peripheral Interface (SPI): ATmega8 microcontroller holds three integrated communication devices.
 - Probes(sensors):-
         - A probe is effectively an elaborate switch, designed to trigger on contact with a component surface, providing accurate, repeatable geometric data. Obtaining and interrogating this data throughout the manufacturing process can help to ensure components remain within conformance limits.
 - Buzzer :-
         - A buzzer or beeper is an audio signaling device, which may be mechanical, electromechanical, or piezoelectric.
         - An arduino buzzer is also called a piezo buzzer. It is basically a tiny speaker that you can connect directly to an Arduino. You can make it sound a tone at a frequency you set. The buzzer produces sound based on reverse of the piezoelectric effect.
 - Seven Segment Display :- 
         - A seven-segment display is a form of electronic display device for displaying decimal numerals that is an alternative to the more complex dot matrix displays. Seven-segment displays are widely used in digital clocks, electronic meters, basic calculators, and other electronic devices that display numerical information.
         - he 7-segment display, also written as “seven segment display”, consists of seven LEDs (hence its name) arranged in a rectangular fashion as shown. Each of the seven LEDs is called a segment because when illuminated the segment forms part of a numerical digit (both Decimal and Hex) to be displayed.
 - transistor :-
         - A transistor is a device that regulates current or voltage flow and acts as a switch or gate for electronic signals. 
         - Transistors consist of three layers of a semiconductor material, each capable of carrying a current. ... A transistor regulates current or voltage flow and acts as a switch or gate for electronic signals.
         - transistor, semiconductor device for amplifying, controlling, and generating electrical signals.
         - we think that BC547 is a normal NPN (Negative-Positive-Negative) junction transistor. 
          
 - Resistors :-
         - A resistor is a passive two-terminal electrical component that implements electrical resistance as a circuit element.
         -  In electronic circuits, resistors are used to reduce current flow, adjust signal levels, to divide voltages, bias active elements, and terminate transmission lines, among other uses.
         - Resistors are common elements of electrical networks and electronic circuits and are ubiquitous in electronic equipment. Practical resistors as discrete components can be composed of various compounds and forms. Resistors are also implemented within integrated circuits.


## 5W and 1H :- 
![5W1H Template](https://user-images.githubusercontent.com/98821876/155528738-ddd4bf00-70d4-4414-8ef4-0b0f1bbc9492.jpg)






## Features:-

 - Easy installation.
 - Low maintenance.
 - Compact elegant design.
 - The Automatic water level controller ensures no overflows or dry running of pump there by saves electricity and water.
 - Avoid seepage of roofs and walls due to overflowing tanks.
 - Fully automatic, saves man power.
 - Consume very little energy, ideal for continuous operation.
 - Automatic water level controller provides you the flexibility to decide for yourself the water levels for operations of pump set.
 - Shows clear indication of water levels in the overhead tank.
 




 1. Power Saver:
    Living in an age where we need to be more conscious of the energy that we use, a water level controller is ideal at saving power. Normally, regulating water levels can consume electricity and wastewater. However, with automatic controllers, the electricity usage is limited as well as less water needed to regulate supply.

 2. Money Saver:
    A water level controller helps save money by limiting the waste of water and electricity. These devices accurately regulate how much energy is used to protect against any unnecessary water/electricity usage. Over time, the money saved is quite substantial.

 3. Automatic:
    Another notable advantage with these devices is that they regulate on their own. Eliminating manual operations with a timer switch, the frustrations of manual monitoring water tanks are minimized. Water levels are maintained at the appropriate levels thanks to the automatic operations of these devices.

 4. Water Maximization:
    On average, water pumps are used more during midday. A water level controller can maximize the water usage provided during midday while automatically lessening the water usage at night.  This results in an appropriate level of water at all times being maintained, while providing you with the maximum use of your water at the appropriate times.

 5. Reliable Electronic Design:
    Addressing the durability problems found in earlier designs, the solid-state electronics in the newer models help to eliminate them. Not only do they help to eliminate the durability issues, but they also create considerable savings of the life span of the unit with an advanced modular design. In order to minimize problem areas of these designs, the only moving parts are the relays. These relays are easily replaced and tested by any skilled operator or electrician while being an inexpensive part.

 6. New Control Minimize Fouling & Deterioration :
    Proving to be less costly, over time, than the original float design for the ‘toilet tank’. The solid-state electronics are designed to minimize volt usage (less than 1 volt). This directly minimizes the mineral fouling, plating, rusting, and deterioration of probes, proving to be safer and more efficient. These factors extend the life span of the controllers significantly, which saves money and energy.

 7. Easy Installation with lcd Monitoring:
   These new solid-state electronics and integrated electronics offer superior performance, hassle-free installation, and lower cost to operate over time when compared to the lifespan of the original design. For continuous monitoring, the integrated firmware and digital dry-contact circuitry easily and quickly connect to the automation systems of a building. Each function of the integrated electronics and relays use LED lights to offer operators the ability to visually scan them in order to verify proper 


 1. Water level controls need to be replaced every 3 years.
 2. The rust, foul and deteriorate
 3. Electronics are usually built separately



 1. Easy installation
 2. Minimal maintenance
 3. Sends an alert to let you know water is too high or too low
 4. Low alarms
 5. Compact design
 6. Save money by using less electricity and water
 7. Can help avoid seepage of roofs and walls due to tanks overflowing
 


 
## Applications :- 
 - Hotels
 - Home apartments
 - Commercial complexes
 - Factories
 - Where cooling towers are used
 - Residential and commercial swimming pools
 - Anywhere water levels need to be controlled
 - In vehicles as a fuel level indicator
 - In huge containers as a liquid level indicator
 - Single phase motor
 - Single phase submersibles
 - Three phase motors
 - Open wells
 - Bore wells
 - Sump Pumps
 - Used to start and stop water pumps 
 - Water level indicator for water tank
 - Automatic water level controller will automatically START the pump set as soon as the water level falls below the predetermined level (usually 1/2 tank) and shall SWITCH OFF    the pump set as soon as tank is full.
 - Liquid level indicator in the huge containers in the companies.
       

