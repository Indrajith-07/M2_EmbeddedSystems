# Implementation

## Code :

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





    
 ## Circuit Diagram :
 
![water_level_indicator_circuit](https://user-images.githubusercontent.com/98821876/157044201-2556f8bb-0863-4658-a6e9-5260bae6f736.png)













## Design of Water Level Indicator Project using AVR Microcontroller : 

  - A constant 5v power supply is given to the microcontroller and rest of the circuit from a battery.
	- The tank has 9 conductive type sensors  embedded into it and 8 wires of sensors out of 9 are connected to transistors and the 9th is connected to 5v+ supply.
	- The use of transistor is it acts as inverter (i.e. in on state gives low voltage at output and in non conducting state gives high voltage at its output), all transistors outputs are connected to PORTB of microcontroller.
	Seven segment display is connected to PORTD. It is connected in common cathode fashion.
	- The Output for the 7th level is not only shown on seven segment display but also indicated with a discontinuous buzzer sound.
	- Output for the 8th level (i.e. tank full condition) is not only shown in seven segment display but also indicated with a continuous buzzer sound.


## Working of Water Level Indicator  : 


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

    
