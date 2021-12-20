# Experiment 3 -  LED Chasing Effect

We often see billboards composed of colorful LEDs. They are constantly changing to form various light effects. 
In this experiment, we compile a program to simulate LED chasing effect.
The long lead of LED is the positive side; short lead is negative.

### Components Required 

1* Arduino Uno Board x1
2* USB Cable x1
3* Led 6
4* Breadboard wire 13
5* 220Ω resistor x3
6* Breadboard x1



# Circuit Diagram

![s5yR0_3102_1627567167](https://user-images.githubusercontent.com/76148902/146768426-eac7b2fb-1681-4f5c-9224-b5d4b05d2ae7.png)


# Code

```
int BASE = 2;  // the I/O pin for the first LED
int NUM = 6;   // number of LEDs
void setup()
{
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     pinMode(i, OUTPUT);   // set I/O pins as output
   }
}
void loop()
{
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     digitalWrite(i, LOW);    // set I/O pins as “low”, turn off LEDs one by one.
     delay(200);        // delay
   }
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     digitalWrite(i, HIGH);    // set I/O pins as “high”, turn on LEDs one by one
     delay(200);        // delay
   }  
}
```

# Output

