# Experiment 4 - Button Controlled LED


### Components Required.

1* Arduino Uno
2* Button switch-1
3* Red M5 LED-1
4* 220ΩResistor-1
5* 10KΩ Resistor-1
6* Breadboard-1
7* Breadboard Jumper Wire-6
8* USB cable-1


# Circuit Diagram

![Ztk6E_3102_1628160172](https://user-images.githubusercontent.com/76148902/148686494-e6599443-be16-43a6-9ed8-04f1d1a9607e.png)


# Code

```
int ledpin=11;// initialize pin 11
int inpin=7;// initialize pin 7
int val;// define val
void setup()
{
pinMode(ledpin,OUTPUT);// set LED pin as “output”
pinMode(inpin,INPUT);// set button pin as “input”
}
void loop()
{
val=digitalRead(inpin);// read the level value of pin 7 and assign if to val
if(val==LOW)// check if the button is pressed, if yes, turn on the LED
{ digitalWrite(ledpin,LOW);}
else
{ digitalWrite(ledpin,HIGH);}
}
```

# Output


