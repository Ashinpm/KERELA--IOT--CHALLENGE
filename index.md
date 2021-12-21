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
make sure code is uploaded without any error to the board.if any error encountred please google the errorcode 🙂 Watch This YouTube Video for More Clarification

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

Watch This YouTube Video for More Clarification
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

Watch This YouTube Video for More Clarification

<iframe width="560" height="315" src="https://www.youtube.com/embed/xIha-fq0PT8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>





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
Press Clr + Shift + M in Arduino Software or go to TOOLS then Click on SERIAL MONITOR to see the output.

> We can see te room temprature on serial monitor


# Experiment 10
# IR Remote Control Using TSOP And Arduino

### Components Required  🗒️

* Arduino Uno  Board
* Infrared Remote Controller(You can use TV Remote or any other remote)
* Infrared Receiver *1
* LED *6
* 220ΩResistor *6
* Breadboard Wire *11

### Circuit Diagram 🧭

![circuit diagram](https://user-images.githubusercontent.com/95163711/146963454-fd8504f1-ae3c-4faf-9e4c-91eea5136560.png)

### About TSOP - IR Receiver Module

![circuit diagram](https://user-images.githubusercontent.com/95163711/146963415-9df4cb29-ebae-4c08-8c3e-add595939c0f.png)


What is an infrared receiver?

The signal from the infrared remote controller is a series of binary pulse code. To avoid the other infrared signal interference during the wireless transmission, the signal is pre-modulated at a specific carrier frequency and then send out by an infrared emission diode. The infrared receiving device needs to filter out other waves and receive signals at that specific frequency and to modulate it back to binary pulse code, known as demodulation.

Working Principle

The built-in receiver converts the light signal it received from the sender into feeble electrical signal. The signal will be amplified by the IC amplifier. After automatic gain control, band-pass filtering, demodulation, wave shaping, it returns to the original code. The code is then input to the code identification circuit by the receiver's signal output pin.

### Program Code 💻
```ino
#include <IRremote.h>
int RECV_PIN = 11;
int LED1 = 2;
int LED2 = 3;
int LED3 = 4;
int LED4 = 5;
int LED5 = 6;
int LED6 = 7;
long on1  = 0x00FF6897;
long off1 = 0x00FF9867;
long on2 = 0x00FFB04F;
long off2 = 0x00FF30CF;
long on3 = 0x00FF18E7;
long off3 = 0x00FF7A85;
long on4 = 0x00FF10EF;
long off4 = 0x00FF38C7;
long on5 = 0x00FF5AA5;
long off5 = 0x00FF42BD;
long on6 = 0x00FF4AB5;
long off6 = 0x00FF52AD;
IRrecv irrecv(RECV_PIN);
decode_results results;
// Dumps out the decode_results structure.
// Call this after IRrecv::decode()
// void * to work around compiler issue
//void dump(void *v) {
//  decode_results *results = (decode_results *)v
void dump(decode_results *results) {
  int count = results->rawlen;
  if (results->decode_type == UNKNOWN) 
    {
     Serial.println("Could not decode message");
    } 
  else 
   {
    if (results->decode_type == NEC) 
      {
       Serial.print("Decoded NEC: ");
      } 
    else if (results->decode_type == SONY) 
      {
       Serial.print("Decoded SONY: ");
      } 
    else if (results->decode_type == RC5) 
      {
       Serial.print("Decoded RC5: ");
      } 
    else if (results->decode_type == RC6) 
      {
       Serial.print("Decoded RC6: ");
      }
     Serial.print(results->value, HEX);
     Serial.print(" (");
     Serial.print(results->bits, DEC);
     Serial.println(" bits)");
   }
     Serial.print("Raw (");
     Serial.print(count, DEC);
     Serial.print("): ");
 for (int i = 0; i < count; i++) 
     {
      if ((i % 2) == 1) {
      Serial.print(results->rawbuf[i]*USECPERTICK, DEC);
     } 
    else  
     {
      Serial.print(-(int)results->rawbuf[i]*USECPERTICK, DEC);
     }
    Serial.print(" ");
     }
      Serial.println("");
     }
void setup()
 {
  pinMode(RECV_PIN, INPUT);   
  pinMode(LED1, OUTPUT);
  pinMode(LED2, OUTPUT);
  pinMode(LED3, OUTPUT);
  pinMode(LED4, OUTPUT);
  pinMode(LED5, OUTPUT);
  pinMode(LED6, OUTPUT);  
  pinMode(13, OUTPUT);
  Serial.begin(9600);
   irrecv.enableIRIn(); // Start the receiver
 }
int on = 0;
unsigned long last = millis();
void loop() 
{
  if (irrecv.decode(&results)) 
   {
    // If it's been at least 1/4 second since the last
    // IR received, toggle the relay
    if (millis() - last > 250) 
      {
       on = !on;
//       digitalWrite(8, on ? HIGH : LOW);
       digitalWrite(13, on ? HIGH : LOW);
       dump(&results);
      }
    if (results.value == on1 )
       digitalWrite(LED1, HIGH);
    if (results.value == off1 )
       digitalWrite(LED1, LOW); 
    if (results.value == on2 )
       digitalWrite(LED2, HIGH);
    if (results.value == off2 )
       digitalWrite(LED2, LOW); 
    if (results.value == on3 )
       digitalWrite(LED3, HIGH);
    if (results.value == off3 )
       digitalWrite(LED3, LOW);
    if (results.value == on4 )
       digitalWrite(LED4, HIGH);
    if (results.value == off4 )
       digitalWrite(LED4, LOW); 
    if (results.value == on5 )
       digitalWrite(LED5, HIGH);
    if (results.value == off5 )
       digitalWrite(LED5, LOW); 
    if (results.value == on6 )
       digitalWrite(LED6, HIGH);
    if (results.value == off6 )
       digitalWrite(LED6, LOW);        
    last = millis();      
irrecv.resume(); // Receive the next value
  }
}

```

### Output 📝

![output](https://user-images.githubusercontent.com/95163711/146963462-399d8e87-c257-4cfe-95ca-7416e103cb99.png)

Watch This YouTube Video for More Clarification

<iframe width="560" height="315" src="https://www.youtube.com/embed/8E3ltjnbV0c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



# Experiment 11
# Potentiometer analog Value Reading Using Arduino

### Components Required  🗒️

* Arduino Uno  Board
* 10K Potentiometer
* Jumper Wire
* Breadboard

### Circuit Diagram 🧭

![circuit diagram](https://user-images.githubusercontent.com/95163711/146965618-427ccc13-f13c-4249-8faf-bae2905f0967.png)

### About Potentiometer
Potentiometer = Variable Resistor. A potentiometer is a three-terminal resistor with a sliding or rotating contact that forms an adjustable voltage divider. Potentiometers are commonly used to control electrical devices such as volume controls on audio equipment

![circuit diagram](https://user-images.githubusercontent.com/95163711/146965609-510eac8a-b0df-4893-a8b9-5ce89abdb7f1.png)

### Program Code 💻
```ino
int potpin=0;// initialize analog pin 0

int ledpin=13;// initialize digital pin 13

int val=0;// define val, assign initial value 0

void setup()

{

pinMode(ledpin,OUTPUT);// set digital pin as “output”

Serial.begin(9600);// set baud rate at 9600

}

void loop()

{

digitalWrite(ledpin,HIGH);// turn on the LED on pin 13

delay(50);// wait for 0.05 second

digitalWrite(ledpin,LOW);// turn off the LED on pin 13

delay(50);// wait for 0.05 second

val=analogRead(potpin);// read the analog value of analog pin 0, and assign it to val

Serial.println(val);// display val’s value

}
```
### Output 📝

![output](https://user-images.githubusercontent.com/95163711/146965628-ef8d5c4c-e5e9-4efa-bcba-6651438c78d0.png)

Watch This YouTube Video for More Clarification

<iframe width="560" height="315" src="https://www.youtube.com/embed/t9DEAreCD3g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


# Experiment 11
# 7 Segment Display & Arduino

### Components Required  🗒️

* Arduino Uno
* 1-digit LED Segment Display x 1
* 220Ω Resistor x 8
* Breadboard
* Jumper Wires 

### Circuit Diagram 🧭

![circuit diagram](https://user-images.githubusercontent.com/95163711/146967454-e944e5ac-52f1-4fb1-b252-b0cabdb57d9b.png)

### About Potentiometer
LED segment display is a semiconductor light-emitting device. Its basic unit is a light-emitting diode (LED). LED segment display can be divided into 7-segment display and 8-segment display according to the number of segments. 8-segment display has one more LED unit ( for decimal point display) than 7-segment one.

![circuit diagram](https://user-images.githubusercontent.com/95163711/146967433-b28ad98c-a40a-4515-8614-edaaba701412.png)
![circuit diagram](https://user-images.githubusercontent.com/95163711/146967443-6110201c-320e-4c36-9df7-87a5c5c1022b.png)

### Program Code 💻
```ino
int a=7;// set digital pin 7 for segment a
int b=6;// set digital pin 6 for segment b
int c=5;// set digital pin 5 for segment c
int d=10;// set digital pin 10 for segment d
int e=11;// set digital pin 11 for segment e
int f=8;// set digital pin 8 for segment f
int g=9;// set digital pin 9 for segment g
int dp=4;// set digital pin 4 for segment dp
void digital_0(void) // display number 5
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(e,HIGH);
digitalWrite(f,HIGH);
digitalWrite(g,LOW);
digitalWrite(dp,LOW);
}
void digital_1(void) // display number 1
{
unsigned char j;
digitalWrite(c,HIGH);// set level as “high” for pin 5, turn on segment c
digitalWrite(b,HIGH);// turn on segment b
for(j=7;j<=11;j++)// turn off other segments
digitalWrite(j,LOW);
digitalWrite(dp,LOW);// turn off segment dp
}
void digital_2(void) // display number 2
{
unsigned char j;
digitalWrite(b,HIGH);
digitalWrite(a,HIGH);
for(j=9;j<=11;j++)
digitalWrite(j,HIGH);
digitalWrite(dp,LOW);
digitalWrite(c,LOW);
digitalWrite(f,LOW);
}
void digital_3(void) // display number 3
{digitalWrite(g,HIGH);
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(dp,LOW);
digitalWrite(f,LOW);
digitalWrite(e,LOW);
}
void digital_4(void) // display number 4
{digitalWrite(c,HIGH);
digitalWrite(b,HIGH);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
digitalWrite(a,LOW);
digitalWrite(e,LOW);
digitalWrite(d,LOW);
}
void digital_5(void) // display number 5
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b, LOW);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(e, LOW);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
}
void digital_6(void) // display number 6
{
unsigned char j;
for(j=7;j<=11;j++)
digitalWrite(j,HIGH);
digitalWrite(c,HIGH);
digitalWrite(dp,LOW);
digitalWrite(b,LOW);
}
void digital_7(void) // display number 7
{
unsigned char j;
for(j=5;j<=7;j++)
digitalWrite(j,HIGH);
digitalWrite(dp,LOW);
for(j=8;j<=11;j++)
digitalWrite(j,LOW);
}
void digital_8(void) // display number 8
{
unsigned char j;
for(j=5;j<=11;j++)
digitalWrite(j,HIGH);
digitalWrite(dp,LOW);
}
void digital_9(void) // display number 5
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(e, LOW);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
}
void setup()
{
int i;// set variable
for(i=4;i<=11;i++)
pinMode(i,OUTPUT);// set pin 4-11as “output”
}
void loop()
{
while(1)
{
digital_0();// display number 0
delay(1000);// wait for 1s
digital_1();// display number 1
delay(1000);// wait for 1s
digital_2();// display number 2
delay(1000); // wait for 1s
digital_3();// display number 3
delay(1000); // wait for 1s
digital_4();// display number 4
delay(1000); // wait for 1s
digital_5();// display number 5
delay(1000); // wait for 1s
digital_6();// display number 6
delay(1000); // wait for 1s
digital_7();// display number 7
delay(1000); // wait for 1s
digital_8();// display number 8
delay(1000); // wait for 1s
digital_9();// display number 9
delay(1000); // wait for 1s
}}

```

### Output 📝

![output](https://user-images.githubusercontent.com/95163711/146967460-aeb435a0-1433-4ab2-b631-5f6479d1f26b.png)




















