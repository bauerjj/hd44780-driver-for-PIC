# hd47780-driver-for-PIC
A Hitachi HD47780 driver for 4-bit/8-bit operation using any PIC microcontroller

For tutorial about setup: http://mcuhq.com/22/hd47780-lcd-driver-for-a-pic

Typical usage:

```
#include "lcd.h"
#include <xc.h>
#include <stdio.h>

void main(){
	// Setup OSSCON and pins here
	// ....
	
	
	initLCD();
	gotoLCD(FIRST_LINE);
	printf("  Hello World");
	gotoLCD(SECOND_LINE);
	printf("** mcuhq.com **");
	// Optional non-printf
	// lcdPrint("  Hello World")
	while(1); // do nothing
}
```
	
