# Experiment 2 -  Traffic Light

In the previous program, we have done the LED blinking experiment with one LED. Now, it’s time to up the stakes and do a bit more complicated experiment-traffic lights.
Actually, these two experiments are similar. While in this traffic lights experiment, we use 3 LEDs with different colors rather than 1 LED

### Components Required 

1* Arduino Uno Board x1 <br>
2* USB Cable x1 <br>
3* Red M5 LED x1 <br>
4* Yellow M5 LED x1 <br>
5* Green M5 LED x1 <br>
6* 220Ω resistor x3 <br>
7* Breadboard x1 <br>
8* Breadboard jumper wires x several <br>


# Circuit Diagram

![yiU1x_3102_1627566759](https://user-images.githubusercontent.com/76148902/146767298-6de33711-4e94-4cdc-a9be-429fad0130d6.png)


# Code

```
int redled =10; // initialize digital pin 8.
int yellowled =7; // initialize digital pin 7.
int greenled =4; // initialize digital pin 4.
void setup()
{
pinMode(redled, OUTPUT);// set the pin with red LED as “output”
pinMode(yellowled, OUTPUT); // set the pin with yellow LED as “output”
pinMode(greenled, OUTPUT); // set the pin with green LED as “output”
}
void loop()
{
digitalWrite(greenled, HIGH);//// turn on green LED
delay(5000);// wait 5 seconds

digitalWrite(greenled, LOW); // turn off green LED
for(int i=0;i<3;i++)// blinks for 3 times
{
delay(500);// wait 0.5 second
digitalWrite(yellowled, HIGH);// turn on yellow LED
delay(500);// wait 0.5 second
digitalWrite(yellowled, LOW);// turn off yellow LED
} 
delay(500);// wait 0.5 second
digitalWrite(redled, HIGH);// turn on red LED
delay(5000);// wait 5 seconds
digitalWrite(redled, LOW);// turn off red LED
}
```

# Output

![2](https://user-images.githubusercontent.com/76148902/147094652-2dfb6a8c-b46a-4528-873f-c534c70f044c.jpg)
