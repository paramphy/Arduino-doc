# LEDs control with Ultrasonic sensor

## Author: Chitrak Roychowdhury

Using sensor the distance of the object is detected and the led will blink accordingly.When the object is far away from the sensor all the LEDs will turn off and when it is just near the sensor all the leds will glow.The Ultrasonic sensor is very popular and used to measure the distance to an object. It comes complete with ultrasonic transmitter and receiver modules. Hc-sr04 transmit high-frequency sound and when an object detects then reflect the signal to echo.

# Components Required

You will need the following components −

- Arduino Uno R3
- 1 x Red LED
- 1 x Green LED
- 2 x Blue LED
- 1 x White LED
- 1 x Yellow LED
- 1 x Orange LED
- 7 x 1kΩ Resistor
- 1 x Ultrasonic Distance Sensor

# Procedure

Follow the circuit diagram and hook up the components on the breadboard as shown in the image given below.

![Imgur](https://i.imgur.com/ODjsU1e.png)


# Arduino Code

```c++
/*
  Contributed by: Chitrak Roychowdhury
  // C++ code*/
const int trig = 12;
const int echo = 13;
const int LED1 = 11;
const int LED2 = 10;
const int LED3 = 9;
const int LED4 = 8;
const int LED5 = 7;
const int LED6 = 6;
const int LED7 = 5;
const int LED8 = 4;
const int LED9 = 3;
const int LED10 = 2;
int duration = 0;
int distance = 0;
void setup()
{
	pinMode(trig , OUTPUT);
	pinMode(echo , INPUT);
	pinMode(LED1 , OUTPUT);
	pinMode(LED2 , OUTPUT);
	pinMode(LED3 , OUTPUT);
	pinMode(LED4 , OUTPUT);
	pinMode(LED5 , OUTPUT);
	pinMode(LED6 , OUTPUT);
	pinMode(LED7 , OUTPUT);
	pinMode(LED8 , OUTPUT);
	pinMode(LED9 , OUTPUT);
	pinMode(LED10 , OUTPUT);
	Serial.begin(9600);
}
void loop() {
	digitalWrite(trig , HIGH);
	delayMicroseconds(1000);
	digitalWrite(trig , LOW);
	duration = pulseIn(echo , HIGH);
	distance = (duration/2) / 28.5 ;
	Serial.println(distance);
  
	if(distance<= 7)
    {
		digitalWrite(LED1, HIGH);
    }
	else {
		digitalWrite(LED1, LOW);
    }
	if ( distance<= 14 )
	{
		digitalWrite(LED2, HIGH); }
	else {
		digitalWrite(LED2, LOW); }
	if ( distance<= 21 )
	{
		digitalWrite(LED3, HIGH); }
	else {
		digitalWrite(LED3, LOW); }
	if ( distance<= 28 )
	{
		digitalWrite(LED4, HIGH); }
	else {
		digitalWrite(LED4, LOW); }
	if ( distance<= 35 )
	{
		digitalWrite(LED5, HIGH); }
	else {
		digitalWrite(LED5, LOW); }
	if ( distance<= 42 )
	{
		digitalWrite(LED6, HIGH); }
	else {
		digitalWrite(LED6, LOW); }
	if ( distance<= 49 )
	{
		digitalWrite(LED7, HIGH); }
	else {
		digitalWrite(LED7, LOW); }
	if ( distance<= 55 )
	{
		digitalWrite(LED8, HIGH); }
	else {
		digitalWrite(LED8, LOW); }
	if ( distance<=60 )
	{
		digitalWrite(LED9, HIGH); }
	else {
		digitalWrite(LED9, LOW); }
	if ( distance<= 65 )
	{
		digitalWrite(LED10, HIGH);
	}
	else {
		digitalWrite(LED10, LOW);
	}
}

```

# Code to Note


# Tinkar Simulation Link

<iframe width="725" height="453" src="https://www.tinkercad.com/things/f2boiQhRNZn-led-control-with-ultrasonic-sensor" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>
