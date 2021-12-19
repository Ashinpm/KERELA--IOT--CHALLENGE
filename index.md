# KERALA-IOT-CHALLENGE [2021-22]


# HELLO ..✋ 

## About Me

### Name 🧑‍🦰    : ASHIN PM
### Status 😈  : B.Tech ECE 3rd year student
### College 🏗️ : IES chittilapilly Thrissur
### From 🚞    : Thrissur , Thalikulam
.........................................................................................................

# KERALA-IOT-CHALLENGE-[2021-22]
# INTRODUCTION
### Foxlab Makerspace in association with GTech - Group of Technology Companies in Kerala is launching our prestigious program “Kerala IoT Challenge 2021”, with a vision to mould 100 IoT experts in Kerala, hosting on the µLearn platform. Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation


## LET'S BEGIN


### What is ARDUINO 
Arduino is an open-source hardware and software company, project, and user community that designs and manufactures single-board microcontrollers and microcontroller kits for building digital devices
orgin - ITALY


# Experiment 1 
## LED Blinking

### Components Required  
* Arduino Uno Board 
* USB Cable 
* LED
* 220 OHM Resistor
* Breadboard 
* Jumper Wires

### Circut Connection
![circuit diagram](https://user-images.githubusercontent.com/91405741/137279765-8a82a34f-1dc0-4afc-9bd3-a31d7f62c428.png)

### Program Code


int ledPin = 10; // define digital pin 10.
void setup()
{
pinMode(ledPin, OUTPUT);// define pin with LED connected as output.
}
void loop()
{
digitalWrite(ledPin, HIGH); // set the LED on.
delay(1000); // wait for a second.
digitalWrite(ledPin, LOW); // set the LED off.
delay(1000); // wait for a second
}
