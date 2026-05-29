# Traffic Light Controller

## Aim
To design a traffic light controller using Arduino.

## Components Used
- Arduino UNO
- LEDs
- Breadboard
- Resistors

## circuit Diagram
![Traffic Light circuit](https://github.com/ayshazara177/traffic-light-controller-/blob/main/Screenshot%202026-05-25%20003327.png?raw=true)

## tinker cad link
[ open tinkercad link ](https://www.tinkercad.com/things/c6mMuS9Noh4-tremendous-amberis-maimu)

## Arduino code
int red=11;
int green=10;
int yellow=9;
  void setup()
  { pinMode(red, OUTPUT);
   pinMode(green, OUTPUT);
   pinMode(yellow, OUTPUT);}
void loop()
{ digitalWrite(red, HIGH);
 digitalWrite(yellow, LOW);
 digitalWrite(green, LOW);
 delay(10000);
 digitalWrite(green, HIGH);
 digitalWrite(red, LOW);
 digitalWrite(yellow, LOW);
 delay(5000);

 digitalWrite(red, LOW);
 digitalWrite(green, LOW);
 for(int i=0;i<3;i++);
 digitalWrite(yellow, HIGH);
 delay(250);
 digitalWrite(yellow, LOW);
 delay(250);}


## Working
The LEDs glow in sequence like a traffic signal.

## Output
The project successfully controls the LEDs automatically.
