/* Copyright (c) 2020 MTHS All rights reserved
 *
 * Created by: Michael Bruneau
 * Created on: Feb 2023
 * This module is a Arduino program that causes a light to blink and cuases the blink delay to increase overtime
*/



// C code

// variables
int blinkDelay = 1000;

// setup
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  // turns on Led then pauses for time = to time delay
  digitalWrite(LED_BUILTIN, HIGH);
  delay(blinkDelay); // Wait for 1000 millisecond(s)
  
  // turnns off Led then pauses for time = to time delay
  digitalWrite(LED_BUILTIN, LOW);
  delay(blinkDelay); // Wait for 1000 millisecond(s)
  
  // increases blink delay by 1000 each loop
  blinkDelay += 1000;
}
