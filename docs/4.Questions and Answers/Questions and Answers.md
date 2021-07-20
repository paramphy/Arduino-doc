# Questions and Answers
 
 
 
 - **What do you mean by open-source hardware? Give an example.**

    Open-source hardware (OSH) consists of physical artifacts of technology designed and offered by the open-design movement.The term usually means that information about the hardware is easily discerned so that others can make it.
 ---

 - **What are the advantages in using Arduino over other microcontroller platforms?**

 ---

 - **Which software is used in Arduino sketch? What is the file extension of the sketch?**
 ---

 - **Which microcontroller is used in Arduino uno? What is the clock speed of this microcontroller?**
 ---

 - **How many digital input/output pins and analog input pins are there in Arduino uno?**
 ---
 - **What reference voltages can be obtained from the Arduino uno board? What is the use of AREF pin?**
 ---

 - **Explain, with an example, the term ‘variables’ in sketch.**
 ---
 - **Explain, with an example, the term ‘functions’ in sketch.**
 ---
 - **What the setup() and loop() functions in sketch are used for?**
 ---
 - **What does the syntax digitalWrite(pin, HIGH) describe?**
 ---
 - **What is the function analogWrite() used for?**
 ---
 - **What is the function Serial.println() used for? Give an example.**
 ---
 - **What sensor is used for measuring the temperature with Arduino? How does the output of the sensor vary with varying temperature?**
 ---
 - **What sensors may be used in the measurement of the period of oscillation of simple pendulum with Arduino? Explain.**
 ---
 - **Write the sketch for blinking LED with delay 5 s.**
 ---
 - **What is Pulse Width Modulation?**
 ---
 - **How many digital and analog pins are there on the UNO board?**
 ---
 - **Explain the setup() and loop() functions.**
 ---
 - **Explain the analogRead() function.**
 ---
 - **What does the command Serial.begin(9600) mean?**
 ---
 - **Explain the delay() function.**
 ---
 - **What does the command analogWrite(127) mean?**
 ---
 - **Explain the pinMode() function.**
 ---
 - **Write down the pin diagram of the sensor LM 35.**
 ---
 - **Write a program to turn on built in LED of the arduino Uno for 1 sec and off for 1 sec.**
 ---
 - **Write a program to read a digital input on the digital pin 2 and prints the result to the serial monitor.**
 ---
 - **Write a program to fade an LED on pin 6.**
 ---
 - **What is a microcontroller? Name three most popular variants of the Arduino microcontroller.**

    A micro-controller is a self contained system with processor, memory and peripherals combined on a single hardware, which is an open source physical computing platform based simple I/O band and development environment.
    
    The three most popular variants of Arduino are
    1. Arduino Uno
    2. Arduino Mega
    3. Arduino Nano
 ---

 - **What are the different components of the CPU of an Arduino Uno microcontroller? Write their functions briefly**

    **Different components of the CPU of an Arduino Uno microcontroller are**

    1. 32 KB flash memory, onto which the programs are stored
    2. 2 KB of RAM, which is the transparent runtime memory.
    3. CPU, which is the brain of the microcontroller.
    4. A non volatile Electrically Erasable Programable Read Only Memory 
    **(EEPROM)** of 1 KB which keeps the data even after device restart and reset.

 ---
 - **Where is the location of the USB interface chip? What is its function?**
 
    ![usbinterfacechip](https://i.imgur.com/Ud5eBU5.jpg)

    
    The Atmega8u2 is a programable USB to UART (Universal Asynchronous Receiver-Transmitter) which converts signals in the USB level to a level compatible with the Arduino Uno Board. 
 ---
 
 - **Can the voltage input to the 6 analog pins in an Arduino Uno microcontroller board go directly to the CPU for processing? What is the maximum voltage that can be accepted by the analog pins?**
 ---
 - **Why cannot the 6 analog pins in an Arduino Uno microcontroller be used to measure current? Which pin among the digital pins of an Arduino Uno microcontroller is connected to the built-in LED?**
  
    The 6 analog pins in an arduino Uno microcontroller can not be used to measure current because they have very high internal resistance.

    Among the digital pins of the arduino Uno microcontroller **PIN 13** in connected to the built-in LED
 ---

 - **What is an Arduino code called? What are the two major sections of an Arduino code?**

    An Arduino Code is called 'Sketch'. An Arduino Code contains two major sections: **setup()** and **loop()**.
    - **setup()** sets up the Arduino hardware, such as specifying which I/O line is going to be used and whether they are inputs or outputs.
    - **loop()** the code under this section is repeated endlessly when the arduino runs.

 ---
 - **What is the resolution of the analog voltage measurement of an Arduino Uno microcontroller and why?**
  
 ---
 - **Which function would you use to time stamp a data output by arduino with relative time? How would you use it?**

    The inbuilt *millis()* function can be used to time stamp a data output by arduino with relative time.

    Returns the number of milliseconds passed since the Arduino board began running the current program. This number will overflow (go back to zero), after approximately 50 days.

    

    This example code prints on the serial port the number of milliseconds passed since the Arduino board started running the code itself.

```c++
unsigned long myTime;

void setup() {
  Serial.begin(9600);
}
void loop() {
  Serial.print("Time: ");
  myTime = millis();

  Serial.println(myTime); // prints time since program started
  delay(1000);          // wait a second so as not to send massive amounts of data
}
```

 ---

