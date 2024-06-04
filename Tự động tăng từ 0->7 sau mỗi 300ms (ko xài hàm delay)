#include <TM1637Display.h>

// define the connections pins
#define CLK 9
#define DIO 10
int num = 0;
unsigned long t=0;
// create a display object of type TM1637Display
TM1637Display display = TM1637Display(CLK, DIO);

void setup() {
  display.clear();
  display.setBrightness(7); 
}

void loop()
{
  if(millis()-t >= 300){
      
      num++; 
      if(num > 7){ num = 0; }
      
      t=millis();
  display.showNumberDec(num);           
  display.clear();
}
}
