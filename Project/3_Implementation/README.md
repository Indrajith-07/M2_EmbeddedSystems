# Implementation

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
