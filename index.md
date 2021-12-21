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


## What is ARDUINO 
![circuit diagram](https://user-images.githubusercontent.com/95163711/146955215-f7cddde3-1601-4d06-ac1d-51dbb45e1f62.png)

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
```ino
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
> the led will blink with delay of 1 second  

congragulation on your first project 😺

### Things to note
make sure code is uploaded without any error to the board.if any error encountred please google the errorcode 🙂 watch the youtube video below to clear all doubts

<iframe width="560" height="315" src="https://www.youtube.com/embed/dnPPoetX0uw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


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

```ino
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

```ino
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
> The LEDs starts turning ON from one end in a sequential manner & after all the LEDs are turned ON, they starts to turn OFF the same way.


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
```ino
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
> LED was Controlled by the switch. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/yqesLSTzf6w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


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
```ino
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
> interfaced buzzer with Arduino.


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
RGB can emit any colour by mixing the 3 basic colours RED GREEN and BLUE. actually it consist of 3 seperate leds for red blue and green packed together in a single case.connect the resistors to the R,G,B terminals respectively.

![circuit diagram](https://user-images.githubusercontent.com/95163711/146745799-fefb9ca2-05f0-4518-8fd7-a5ae4be4de90.png)

### Program Code 💻
```ino
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
> interfaced RGB with Arduino.


# Experiment 7
# LDR Light Sensor & Arduino

### Components Required  🗒️

* Arduino Uno
* 220Ω Resistor*1
* 10KΩ Resistor*1
* Photo Resistor (LDR Sensor)
* jumper wire
* Red M5 LED

### Circuit Diagram 🧭


![circuit diagram](https://user-images.githubusercontent.com/95163711/146747611-f68854d3-308f-4a32-a54e-189b3958d75d.png)

### About LDR Light Sensor
Photo Resistor (Photovaristor) is a resistor whose resistance varies from different incident light strength. It's based on the photoelectric effect of semiconductor. If the incident light is intense, its resistance reduces; if the incident light is weak, the resistance increases.

![circuit diagram](https://user-images.githubusercontent.com/95163711/146747626-da15340f-e361-49f3-baab-0ff439118d7f.png)

### Program Code 💻
```ino
int potpin=0;// initialize analog pin 0, connected with photovaristor

int ledpin=11;// initialize digital pin 11, 

int val=0;// initialize variable val

void setup()

{

pinMode(ledpin,OUTPUT);// set digital pin 11 as “output”

Serial.begin(9600);// set baud rate at “9600”

}

void loop()

{

val=analogRead(potpin);// read the value of the sensor and assign it to val

Serial.println(val);// display the value of val

analogWrite(ledpin,val/4);// set up brightness（maximum value 255）

delay(10);// wait for 0.01 

}

```

### Output 📝
![output](https://user-images.githubusercontent.com/95163711/146748282-d95608d3-1aca-4e8a-80cf-a2952173af66.png)

> interfaced LDR with Arduino.


# Experiment 8
# Flame Detector

### Components Required  🗒️

* Arduino Uno
* Flame Sensor 
* Buzzer
* 10K Resistor 
* Jumper Wire*6
* USB cable

### Circuit Diagram 🧭


![circuit diagram](https://user-images.githubusercontent.com/95163711/146955949-1d11f6c0-c47d-43f6-a2ef-cee03e060766.png)

### About IR sensor
We are using Infrared Receiver (IR )for detecting Flame.The emitter is an IR LED and the detector is an IR photodiode. The IR photodiode is sensitive to the IR light emitted by an IR LED. The photo-diode's resistance and output voltage change in proportion to the IR light received. This is the underlying working principle of the IR sensor.

![circuit diagram](https://user-images.githubusercontent.com/95163711/146955253-2e8d02b2-a2dc-4034-8f5d-8e9f0fb15708.png)



### Program Code 💻
```ino
int flame=0;// select analog pin 0 for the sensor

int Beep=9;// select digital pin 9 for the buzzer

int val=0;// initialize variable

 void setup() 
 
{

  pinMode(Beep,OUTPUT);// set LED pin as “output”
  
 pinMode(flame,INPUT);// set buzzer pin as “input”
 
 Serial.begin(9600);// set baud rate at “9600”
 
 } 
 
void loop() 

{ 

  val=analogRead(flame);// read the analog value of the sensor 
  
  Serial.println(val);// output and display the analog value
  
  if(val>=600)// when the analog value is larger than 600, the buzzer will buzz
  
  {  
  
   digitalWrite(Beep,HIGH); 
   
   }else 
   
   {  
   
     digitalWrite(Beep,LOW); 
     
    }
    
   delay(500); 
   
}
```

### Output 📝
![output](https://user-images.githubusercontent.com/95163711/146955957-e2c059d2-8ab9-42b2-aaf3-e9144ebccd13.png)

> Flame detector will detect the presence of fire and triggers the buzzer.

# Experiment 9
# Thermometer 

### Components Required  🗒️

* Arduino Uno  Board
* LM35 Temprature sensor
* Breadboard
* Breadboard Jumper Wire

### Circuit Diagram 🧭


![circuit diagram](https://user-images.githubusercontent.com/95163711/146960026-4b6e00b3-3130-42ba-bd11-d183ecd27a1b.png)

### About LM35 sensor
![circuit diagram](https://user-images.githubusercontent.com/95163711/146959998-c3ae6922-4aaa-4bab-96c3-4f4a5afe4cb9.png)

LM35 is a common and easy-to-use temperature sensor.LM35 is a widely used temperature sensor with many different package types. At room temperature, it can achieve the accuracy of ±1/4°C without additional calibration processing.LM35 temperature sensor can produce different voltage by different temperatureWhen temperature is 0 ℃, it outputs 0V; if increasing 1 ℃, the output voltage will increase 10 mv.


### Program Code 💻
```ino
int potPin = 0; // initialize analog pin 0 for LM35 temperature sensor

void setup()

{

Serial.begin(9600);// set baud rate at”9600”

}

void loop()

{

int val;// define variable

int dat;// define variable

val=analogRead(0);// read the analog value of the sensor and assign it to val

dat=(125*val)>>8;// temperature calculation formula

Serial.print("Tep");// output and display characters beginning with Tep

Serial.print(dat);// output and display value of dat

Serial.println("C");// display “C” characters

delay(500);// wait for 0.5 second

}

```

### Output 📝
![output](https://user-images.githubusercontent.com/95163711/146960047-ac269a42-a60c-4406-bd83-23e119526183.png)

### *NOTE* 
Press Clr + Shift + M in Arduino Software or got to TOOLS then Click on SERIAL MONITOR to see the output.

> We can see te room temprature on serial monitor





















