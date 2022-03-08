# WATER LEVEL INDICATOR 

## [ 1 ] Introduction and Requirements

## 1.1 :- Overview

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
## 1.2 :- Block Diagram
![Blockdiagram](https://user-images.githubusercontent.com/98821876/155511413-d8af4434-e87a-4393-be53-94ac591fc427.png)
=======


## 1.3 :- High Level Requirement
 
-----------------------------------------------------------------------------------------------
| Req ID  |    Description         |
|-------|--------------------------|
|  HL_01    | if water level is 8 or Full   Display 8 And Buzzer     | 
|-------|--------------------------|
|  HL_02    | if water level is 7         Display 7 And Buzzer   |   
|-------|--------------------------|
|  HL_03    | if water level is 6         Display 6 And Buzzer    | 
|-------|--------------------------|
|  HL_04    | if water level is 5         Display 5 And Buzzer    |  
|-------|--------------------------|
|  HL_05    | if water level is 4         Display 4 And Buzzer     |  
|-------|--------------------------|
|  HL_06    | if water level is 3         Display 3 And Buzzer     |  
|-------|--------------------------|
|  HL_07    | if water level is 2         Display 2 And Buzzer     | 
|-------|--------------------------|
|  HL_08    | if water level is 1         Display 1 And Buzzer     | 
|-------|--------------------------|
|  HL_09    | if water level is 0         Display 0 And Buzzer     | 

 


 ## 1.4 :- Low Level Requirements 
 
 -----------------------------------------------------------------------------------------------
| Req ID  |    Description         |
|-------|--------------------------|
|  LL_01    | Detect water level at Full       | 
|-------|--------------------------|
|  LL_02    | Detect water level at intermediate levels            |   
|-------|--------------------------|
|  LL_03    | Detect water level at empty               | 
|-------|--------------------------|




## 1.5 :- Components Required 

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


## 1.6 :- 5W and 1H 
![5W1H Template](https://user-images.githubusercontent.com/98821876/155528738-ddd4bf00-70d4-4414-8ef4-0b0f1bbc9492.jpg)


## 1.7 :- SWOT Analysis 
 ![swot](https://user-images.githubusercontent.com/98821876/155536695-7c6db3e8-2682-4617-8d15-96153fd2c668.png)




## 1.8 :- Features

 - Easy installation.
 - Low maintenance.
 - Compact elegant design.
 - The Automatic water level controller ensures no overflows or dry running of pump there by saves electricity and water.
 - Avoid seepage of roofs and walls due to overflowing tanks.
 - Fully automatic, saves man power.
 - Consume very little energy, ideal for continuous operation.
 - Automatic water level controller provides you the flexibility to decide for yourself the water levels for operations of pump set.
 - Shows clear indication of water levels in the overhead tank.
 


## 1.9 :- Advantages 

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


## 1.10 :- Disadvantages 

 1. Water level controls need to be replaced every 3 years.
 2. The rust, foul and deteriorate
 3. Electronics are usually built separately


## 1.11 :- Benefits 

 1. Easy installation
 2. Minimal maintenance
 3. Sends an alert to let you know water is too high or too low
 4. Low alarms
 5. Compact design
 6. Save money by using less electricity and water
 7. Can help avoid seepage of roofs and walls due to tanks overflowing
 



## 1.12 :- Applications  

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
       




# [ 2 ] :- ARCHITECTURE


## 2.1 :- Block Diagram  
      
![Blockdiagram](https://user-images.githubusercontent.com/98821876/155734711-4200322a-4ec8-49e5-b528-4a742e61ce4b.png)



## 2.2 :- Flowchart  

![flowchart_atmega8](https://user-images.githubusercontent.com/98821876/155734563-68d801e9-2b82-4173-8913-3f01866ff838.jpg)


## 2.3 :- Structural Diagram 
  ###  2.3.1 : Class diagramm 
  ![Class_atmega8_](https://user-images.githubusercontent.com/98821876/155734830-4e706466-9ccf-4e7f-a006-546292ececbb.png)
  
  ###  2.3.2 : Component diagram :
  ![component_atmega8](https://user-images.githubusercontent.com/98821876/155738826-e3f67f1c-a105-4978-84c3-e2a5641638b4.png)


## 2.4 :- Behaviour Diagram 
  ###  2.4.1 : Sequence diagram 
  ![Sequence_atmega8](https://user-images.githubusercontent.com/98821876/155734971-c9144c30-ff7b-4882-8cef-3f09cf17b615.png)
  
  ### 2.4.2 : Circuit Diagram 
  ![water_level_indicator_circuit](https://user-images.githubusercontent.com/98821876/157054962-89019cf0-4866-4aef-8994-98171df56ae2.png)




# [ 3 ] Implementation

## 3.1 :- Code 

    #define  F_CPU 8000000UL
    #include <avr/io.h>
    #include <util/delay.h>
    
    int main(void)
    {
      DDRB = 0x00;	// PORTB pins as input
	  DDRD = 0xff;	// PORTD as output
	  DDRC = 0x01;		// Buzzer
	  unsigned char seg[10] = {0x3f,0x06,0x5b,0x4f,0x66,0x6d,0x7d,0x07,0x7f,0x67};
	
        while(1)
        {
            if((PINB & 0xff)==0x00)			// 8th probe, Tank full	
		{
			PORTC = 0x01;
			PORTD = seg[8];
		}
		else if((PINB & 0xff)==0x01)		// 7th probe
		{		
			PORTC = 0x01;
			_delay_ms(500);
			PORTC = 0x00;
			_delay_ms(500);
			PORTD = seg[7];
		}
		else if((PINB & 0xff)==0x03)		// 6th probe
		{		
			PORTC = 0x00;
			PORTD = seg[6];
		}
		else if((PINB & 0xff)== 0x07)		// 5th probe
		{		
			PORTC = 0x00;
			PORTD = seg[5];
		}
		else if((PINB & 0xff)== 0x0f)		// 4th probe
		{		
			PORTC = 0x00;
			PORTD = seg[4];
		}
		else if((PINB & 0xff)==0x1f)		// 3rd probe 
		{		
			PORTC = 0x00;
			PORTD = seg[3];
		}
		else if((PINB & 0xff) == 0x3f)		// 2nd probe
		{		
			PORTC = 0x00;
			PORTD = seg[2];
		}	
		else if((PINB & 0xff) == 0x7f)		// 1st probe
		{		
			PORTC = 0x00;
			PORTD = seg[1];
		}	
		else                                // Tank empty
		{
			PORTC = 0x00;
			PORTD = seg[0];
		}					
        } 
    }





    
 ## 3.2 :- Schematic diagram 
 
![water_level_indicator_circuit](https://user-images.githubusercontent.com/98821876/157055385-86e49a74-1883-4893-87b6-aa280a6c8e48.png)














## 3.3 :- Design of Water Level Indicator Project using AVR Microcontroller 

   - A constant 5v power supply is given to the microcontroller and rest of the circuit from a battery.
   - The tank has 9 conductive type sensors  embedded into it and 8 wires of sensors out of 9 are connected to transistors and the 9th is connected to 5v+ supply.
   - The use of transistor is it acts as inverter (i.e. in on state gives low voltage at output and in non conducting state gives high voltage at its output), all transistors        outputs are connected to PORTB of microcontroller.
   - Seven segment display is connected to PORTD. It is connected in common cathode fashion.
   - The Output for the 7th level is not only shown on seven segment display but also indicated with a discontinuous buzzer sound.
   - Output for the 8th level (i.e. tank full condition) is not only shown in seven segment display but also indicated with a continuous buzzer sound.


## 3.4 :- Working of Water Level Indicator  


   - The operation of this project is very simple and can be understood easily. In our project “water level indicator”   there are 3 main conditions:

	 - There is no water available in the source tank.
	 - Intermediate level i.e. either of 3rd to 7th level.
	 - There is ample amount of water available in the source tank.


CONDITION 1: Water not available

   - When the tank is empty there is no conductive path between any of the 8 indicating probes and the common probe     (which is connected to 5v+ supply) so the transistor base emitter region will not have sufficient biasing voltage hence it remains in cut off region and the output across its collector will be Vc approximately 4.2v.
 
   - As in this case the microcontroller is used in the active low region (which means it considers 0-2 volts for HIGH and 3-5 volts for LOW) now the output of transistor which is 4.2v approximately will be considered as LOW by the microcontroller and hence the default value given by microcontroller to the seven segment display is 0 which indicates as the tank is empty.

CONDITION 2: Intermediate levels

   - Now as the water starts filling in the tank a conductive path is established between the sensing probes and the common probe and the corresponding transistors get sufficient biasing at their base, they starts conducting and now the outputs will be Vce (i.e. 1.2v-1.8v) approximately which is given to microcontroller.

   - Here the microcontroller is programmed as a priority encoder which detects the highest priority input and displays corresponding water level in the seven segment display.

   - In this project while the water level reaches the 7th level i.e. last but one level along with display in seven segment a discontinuous buzzer is activated which warns user that tank is going to be full soon.

CONDITION 3: Water full

   - When the tank becomes full, the top level probe gets the conductive path through water and the corresponding transistor gets into conduction whose output given to microcontroller with this input microcontroller not only displays the level in seven segment display but also activates the continuous buzzer by which user can understand that tank is full and can switch off the motor and save water.

    
