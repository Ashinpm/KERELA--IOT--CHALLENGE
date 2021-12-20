# **KERALA-IOT-CHALLENGE [2021-22]**



# *HELLO ...✋* 

## About Me 

### Name 🧑‍🦰    : ASHIN PM
### Status 😈  : B.Tech ECE 3rd year student
### College 🏗️ : IES chittilappilly Thrissur
### From 🚞    : Thrissur , Thalikulam
.........................................................................................................

# **KERALA-IOT-CHALLENGE-[2021-22]**
.........................................................................................................................................................
# INTRODUCTION
### Foxlab Makerspace in association with GTech - Group of Technology Companies in Kerala is launching our prestigious program “Kerala IoT Challenge 2021”, with a vision to mould 100 IoT experts in Kerala, hosting on the µLearn platform. Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation


## LET'S BEGIN


### What is ARDUINO 
Arduino is an open-source hardware and software company, project, and user community that designs and manufactures single-board microcontrollers and microcontroller kits for building digital devices
orgin - ITALY.
For More
click [here](https://www.arduino.cc/en/Guide/Introduction)


# Experiment 1 
# LED Blinking


### Components Required  🗒️
* Arduino Uno Board 
* USB Cable 
* LED
* 220 OHM Resistor
* Breadboard 
* Jumper Wires


### Circut Connection 🧭
![circuit diagram](https://user-images.githubusercontent.com/91405741/137279765-8a82a34f-1dc0-4afc-9bd3-a31d7f62c428.png)



### Program Code 💻
```
int ledPin = 10; // define digital pin 10

void setup()

{

pinMode(ledPin, OUTPUT); // LED connected as output

}

void loop()

{

digitalWrite(ledPin, HIGH); // LED on

delay(1000); // wait for a second

digitalWrite(ledPin, LOW); // LED off

delay(1000); // wait for a second

}
```
### Output 📝
the led will blink with delay of 1 second  

congragulation on your first project 😺

### Things to note
make sure code is uploaded without any error to the board.if any error encountred please google the errorcode 🙂




# Experiment 2
# Traffic Light

### Components Required  🗒️
* Arduino board 
* USB cable 
* Red M5 LED
* Yellow M5 LED
* Green M5 LED
* 220Ω resistor x 3

### Circut Connection 🧭

![circuit diagram](https://user-images.githubusercontent.com/91405741/137288387-e85f8db9-ae97-49d0-888d-a2fc15e4c496.png)

### Program Code 💻

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
### Output 📝

> In Traffic light, the green LED blink about 5 second, then it is turnoff. Then the yellow LED blinks 3 times with a time interval of 0.5 second.Then the red LED blink about 5 seconds. 



# Experiment 3
# LED Chasing Effect 


### Components Required  🗒️

* Led x6
* Arduino board 
* 220Ω resistor x6
* Breadboard 
* wires

### Circuit Diagram 🧭



![circuit diagram](https://user-images.githubusercontent.com/91405741/137292096-feb60c91-1a9a-474b-a596-300285f7b011.png)


### Program Code 💻

```
int BASE = 2;  // the I/O pin for the first LED

int NUM = 6;   // number of LEDs

void setup()

{

   for (int i = BASE; i < BASE + NUM; i++) 
   
   {
   
     pinMode(i, OUTPUT);   // set I/O pins as output
     
   }
   
}

void loop()

{

   for (int i = BASE; i < BASE + NUM; i++) 
   
   {
   
     digitalWrite(i, LOW);    // set I/O pins as “low”, turn off LEDs one by one.
     
     delay(200);        // delay
     
   }
   
   for (int i = BASE; i < BASE + NUM; i++) 
   
   {
   
     digitalWrite(i, HIGH);    // set I/O pins as “high”, turn on LEDs one by one
     
     delay(200);        // delay
     
   }  
   
}

```

### Output 📝
>The LEDs starts turning ON from one end in a sequential manner & after all the LEDs are turned ON, they starts to turn OFF the same way.


# Experiment 4
# Button Controlled LED

### Components Required  🗒️

* Arduino Uno
* Button switch
* Red M5 LED
* 220ΩResistor
* 10KΩ Resistor
* Breadboard
* Jumper Wire

### Circuit Diagram 🧭

![circuit diagram](https://user-images.githubusercontent.com/95163711/146739094-1b20ee7b-072f-47ce-9f9a-dbca058b613f.png)

### Program Code 💻
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

### Output 📝
LED was Controlled by the switch. 


# Experiment 5
# Buzzer & Arduino

### Components Required  🗒️

* Arduino Uno
* Buzzer
* Breadboard
* Jumper Wire


### Circuit Diagram 🧭

![circuit diagram](https://user-images.githubusercontent.com/95163711/146742939-32ba93e5-6980-438b-a892-2784fb76fd42.png)

### Program Code 💻
```
int buzzer=8;// initialize digital IO pin that controls the buzzer

void setup() 

{ 

  pinMode(buzzer,OUTPUT);// set pin mode as “output”
  
} 

void loop() 

{

digitalWrite(buzzer, HIGH); // produce sound

}

```

### Output 📝
interfaced buzzer with Arduino


# Experiment 6
# RGB LED & Arduino

### Components Required  🗒️

* Arduino Uno
* USB Cable 
* RGB LED 
* Resistor 220 ohm
* jumper wire

### Circuit Diagram 🧭

![circuit diagram](https://user-images.githubusercontent.com/95163711/146744513-1f2a5c9e-800d-41d5-863b-f07b9a1adaed.png)

### About RGB
RGB can emit any colour by mixing the 3 basic colours RED GREEN and BLUE. actually it consist of 3 seperate leds for red blue and green packed together in a single case.connect the resistors to the R,G,B terminals respectively

![circuit diagram](https://user-images.githubusercontent.com/95163711/146745799-fefb9ca2-05f0-4518-8fd7-a5ae4be4de90.png)

### Program Code 💻
```
int redpin = 11; //select the pin for the red LED

int bluepin =10; // select the pin for the blue LED

int greenpin =9;// select the pin for the green LED

int val;

void setup() {

  pinMode(redpin, OUTPUT);
  
  pinMode(bluepin, OUTPUT);
  
  pinMode(greenpin, OUTPUT);
  
  Serial.begin(9600);
  
}

void loop() 

{

for(val=255; val>0; val--)

  {
  
   analogWrite(11, val);
   
   analogWrite(10, 255-val);
   
   analogWrite(9, 128-val);
   
   delay(1); 
   
  }
  
for(val=0; val<255; val++)

  {
  
   analogWrite(11, val);
   
   analogWrite(10, 255-val);
   
   analogWrite(9, 128-val);
   
   delay(1); 
   
  }
  
 Serial.println(val, DEC);
 
}

```

### Output 📝
interfaced RGB with Arduino




















