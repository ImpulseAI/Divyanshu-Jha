## Dual Axis Solar Sun Tracker ##
###### _By Divyanshu Jha_ ######

___

### __Project template__ ###

1. [Introduction](#Introduction)
    * (i) [Purpose](#Purpose)
    * (ii) [Scope](#Scope)
    * (iii) [Definition](#Definition)
1. [Overall Description](#Overall-Description)
    * (i) [Arduino UNO Microcontroller](#Arduino-UNO-Microcontroller)
    * (ii) [LDRs](#LDRs)
    * (iii) [Servo Motors](#Servo-Motors)
1. [Operation](#Operation)
1. [Materials Required](#Materials-Required)
1. [Code](#Code)
1. [Conclusion](#Conclusion)
1. [License](#License)

___
### __Introduction__ ###

#### _Purpose_ ####
A typical solar panel converts only 30 to 40 percent of the incident solar irradiation into electrical
energy. Thus to get a constant output, an automated system is required which should be capable to
constantly rotate the solar panel. The Sun Tracking System (STS) was made as a prototype to solve the
problem, mentioned above. It is completely automatic and keeps the panel in front of sun until that is
visible. The unique feature of this system is that instead of taking the earth as its reference, it takes the
sun as a guiding source. Its active sensors constantly monitor the sunlight and rotate the panel towards
the direction where the intensity of sunlight is maximum. With the rapid increase in population and
economic development, the problems of the energy crisis and global warming effects are today a
cause for increasing concern. The utilization of renewable OPEN ACCESS Sensors 2013, 13 3158
energy resources is the key solution to these problems. Solar energy is one of the primary sources of
clean, abundant and inexhaustible energy, that not only provides alternative energy resources, but
also improves environmental pollution. The most immediate and technologically attractive use of
solar energy is through photovoltaic conversion. The physics of the PV cell (also called solar cell) is
very similar to the classical p-n junction diode. The PV cell converts the sunlight directly into direct
current (DC) electricity by the photovoltaic effect. A PV panel or module is a packaged
interconnected assembly of PV cells. In order to maximize the power output from the PV panels, one
needs to keep the panels in an optimum position perpendicular to the solar radiation during the day.
As such, it is necessary to have it equipped with a Sun tracker. Compared to a fixed panel, a mobile
PV panel driven by a Sun tracker may boost consistently the energy gain of the PV panel
___
#### _Scope_ ####
* It can be used for small and medium scale power generations.
* It can be used for power generation at remote places where power lines are not accessible.
* It can be used for domestic and industrial power backup sytem.
* Solar radiation Tracker has played a vital role in increasing the efficiency of solar 
panels in recent years, thus proving to be a better technological achievement. The
vital importance of a dual axis solar tracker lies in its better efficiency and
sustainability to give a better output compared to a fived solar panel or a single axis
solar tracker. The tracking system is designed such that it can trap the solar energy in
all possible directions
___
#### _Definition_ ####
A Solar tracker is an automated solar panel which actually follows the sun to get maximum power.
The primary benefit of a tracking system is to collect solar energy for the longest period of the day,
and with the most accurate alignment as the Sun’s position shifts with the seasons.Dual Axis Tracker
have two different degrees through which they use as axis of rotation. The dual axis are usually at a
normal of each rotate both east to west (zenithal) and north to south. Solar tracking is the most
appropriate technology to enhance the electricity production of a PV system. To achieve a high
degree of tracking accuracy, several approaches have been widely investigated. Generally, they can
be classified as either open-loop tracking types based on solar movement mathematical models or
closed-loop tracking types using sensor-based feedback controllers . In the open-loop tracking
approach, a tracking formula or control algorithm is used. Referring to the literature , the
azimuth and the elevation angles of the Sun were determined by solar movement models or
algorithms at the given date, time and geographical information. The control algorithms were
executed in a microprocessor controller . In the closed-loop tracking approach, various active
sensor devices, such as charge couple devices (CCDs)  or light dependent resistors (LDRs)
were utilized to sense the Sun’s position and a feedback error signal was then generated
to the control system to continuously receive the maximum solar radiation on the PV panel. This
paper proposes an empirical research approach on this issue. Solar tracking approaches can be
implemented by using single-axis schemes, and dual-axis structures for higher accuracy
___
### __Overall Description__ ###

#### Arduino UNO Microcontroller ####

__Arduino__ is an open source, computer hardware and software company, project, and user
community that designs and manufactures microcontroller kits for building digital devices and
interactive objects that can sense and control objects in the physical world. The project's
products are distributed as open-source hardware and software, which are licensed under
the GNU Lesser General Public License (LGPL) or the GNU General Public
License (GPL) permitting the manufacture of Arduino boards and software distribution by
anyone. Arduino boards are available commercially in preassembled form, or as do-ityourself
kits.
Arduino board designs use a variety of microprocessors and controllers. The boards are
equipped with sets of digital and analog input/output (I/O) pins that may be interfaced to
various expansion boards (shields) and other circuits. The boards feature serial
communications interfaces, including Universal Serial Bus (USB) on some models, which are
also used for loading programs from personal computers. The microcontrollers are typically
programmed using a dialect of features from the programming languages C and C++. In
addition to using traditional compiler toolchains, the Arduino project provides an integrated
development environment (IDE) based on the Processing language project.
Arduino/Genuino Uno:- is a microcontroller board based on the ATmega328P. It has 14 digital
input/output pins (of which 6 can be used as PWM outputs), 6 analog inputs, a 16 MHz quartz crystal,
a USB connection, a power jack, an ICSP header and a reset button. It contains everything needed to
support the microcontroller; simply connect it to a computer with a USB cable or power it with a ACto-
DC adapter or battery to get started.. You can tinker with your UNO without worring too much
about doing something wrong, worst case scenario you can replace the chip for a few Rupees and start
over again.
___
#### LDRs ####
A __Light Dependent Resistor (LDR)__ or a photo resistor is a device whose resistivity is a function of
the incident electromagnetic radiation. Hence, they are light sensitive devices. They are also called as
photo conductors, photo conductive cells or simply photocells. They are made up
of semiconductor materials having high resistance. A photoresistor is made of a high
resistance semiconductor. In the dark, a photoresistor can have a resistance as high as
several megohms (MΩ), while in the light, a photoresistor can have a resistance as low as a
few hundred ohms. If incident light on a photoresistor exceeds a
certain frequency, photons absorbed by the semiconductor give bound electrons enough
energy to jump into the conduction band. The resulting free electrons (and
their hole partners)conduct electricity, thereby lowering resistance. The resistance range and
sensitivity of a photoresistor can substantially differ among dissimilar devices. Moreover,
unique photoresistors may react substantially differently to photons within certain wavelength
bands.
___
#### Servo Motors ####
A __servomotor__ is a rotary actuator or linear actuator that allows for precise control of angular
or linear position, velocity and acceleration. It consists of a suitable motor coupled to a
sensor for position feedback. It also requires a relatively sophisticated controller, often a
dedicated module designed specifically for use with servomotors.
Servomotors are not a specific class of motor although the term servomotor is often used to
refer to a motor suitable for use in a closed-loop control system.
A servomotor is a closed-loop servomechanism that uses position feedback to control its
motion and final position. The input to its control is a signal (either analogue or digital)
representing the position commanded for the output shaft.
The motor is paired with some type of encoder to provide position and speed feedback. In
the simplest case, only the position is measured. The measured position of the output is
compared to the command position, the external input to the controller. If the output position
differs from that required, an error signal is generated which then causes the motor to rotatein 
either direction, as needed to bring the output shaft to the appropriate position. As the
positions approach, the error signal reduces to zero and the motor stops.
The very simplest servomotors use position-only sensing via a potentiometer and bang-bang
control of their motor; the motor always rotates at full speed (or is stopped). This type of
servomotor is not widely used in industrial motion control, but it forms the basis of the simple
and cheap servos used for radio-controlled models.
More sophisticated servomotors use optical rotary encoders to measure the speed of the
output shaft and a variable-speed drive to control the motor speed. Both of these
enhancements, usually in combination with a PID control algorithm, allow the servomotor to
be brought to its commanded position more quickly and more precisely, with
less overshooting.
___

#### __Operation__ ####
1. LDRs are used as the main light sensors. Two servo motors are fixed to the structure that holds
the solar panel. The program for Arduino is uploaded to the microcontroller. The working of
the project is as follows.
1. LDRs sense the amount of sunlight falling on them. Four LDRs are divided into top, bottom,
left and right. 
1. For east – west tracking, the analog values from two top LDRs and two bottom LDRs are
compared and if the top set of LDRs receive more light, the vertical servo will move in that
direction.
1. If the bottom LDRs receive more light, the servo moves in that direction.
1. For angular deflection of the solar panel, the analog values from two left LDRs and two right
LDRs are compared. If the left set of LDRs receive more light than the right set, the horizontal
servo will move in that direction. 
1. If the right set of LDRs receive more light, the servo moves in that direction. 

![CD](CD.jpg)
___
### __Materials Required__ ###

| __MATERIALS__ | __PRICE__ |
|:------:|:------:|
| ```Arduino UNO``` | ₹ 450 |
| ```6v 100ma Mini Solar Pannel``` | ₹ 400 |
| ```Soldering Iron``` | ₹ 320 |
| ```20W Hot Glue Gun``` | ₹ 210 |
| ```Foam Board Sheet``` | ₹ 170 |
| ```Wood Glue``` | ₹ 200 |
| ```Detail Pen Knife``` | ₹ 180 |
| ```Jumper Wire``` | ₹ 210 |
| ```Servo Motor``` | ₹ 265 |
| ```Breadboard``` | ₹ 170 |
| ```LDR Sensor``` | ₹ 70 |
| ```100ohm Resistors``` | ₹ 150 |
| ```Wire``` | ₹ 300 |
| ```PCB``` | ₹ 70 |
| | |
| __Total__ | ₹ 3165 |
___

### __Code__ ###
```js
#include <Servo.h>
//defining Servos
Servo servohori;
int servoh = 0;
int servohLimitHigh = 160;
int servohLimitLow = 20;

Servo servoverti; 
int servov = 0; 
int servovLimitHigh = 160;
int servovLimitLow = 20;
//Assigning LDRs
int ldrtopl = 2; //top left LDR green
int ldrtopr = 1; //top right LDR yellow
int ldrbotl = 3; // bottom left LDR blue
int ldrbotr = 0; // bottom right LDR orange

 void setup () 
 {
  servohori.attach(10);
  servohori.write(0);
  servoverti.attach(9);
  servoverti.write(0);
  delay(500);
 }

void loop()
{
  servoh = servohori.read();
  servov = servoverti.read();
  //capturing analog values of each LDR
  int topl = analogRead(ldrtopl);
  int topr = analogRead(ldrtopr);
  int botl = analogRead(ldrbotl);
  int botr = analogRead(ldrbotr);
  // calculating average
  int avgtop = (topl + topr) / 2; //average of top LDRs
  int avgbot = (botl + botr) / 2; //average of bottom LDRs
  int avgleft = (topl + botl) / 2; //average of left LDRs
  int avgright = (topr + botr) / 2; //average of right LDRs

  if (avgtop < avgbot)
  {
    servoverti.write(servov +1);
    if (servov > servovLimitHigh) 
     { 
      servov = servovLimitHigh;
     }
    delay(10);
  }
  else if (avgbot < avgtop)
  {
    servoverti.write(servov -1);
    if (servov < servovLimitLow)
  {
    servov = servovLimitLow;
  }
    delay(10);
  }
  else 
  {
    servoverti.write(servov);
  }
  
  if (avgleft > avgright)
  {
    servohori.write(servoh +1);
    if (servoh > servohLimitHigh)
    {
    servoh = servohLimitHigh;
    }
    delay(10);
  }
  else if (avgright > avgleft)
  {
    servohori.write(servoh -1);
    if (servoh < servohLimitLow)
     {
     servoh = servohLimitLow;
     }
    delay(10);
  }
  else 
  {
    servohori.write(servoh);
  }
  delay(50);
}
```
### __Conclusion__ ###
As dual-axis tracking generates 40% more power from each panel, you can achieve the same
power output with fewer panels, frames and so on, which reduces a project's upfront costs and
offsets to a great extent the additional cost for tracking hardware. On the other hand, you can
use the same number of panels as originally planned and generate 40% more power and higher
revenues. This reduces the project's payback time and also increases the overall return on
investment (ROI), depending on the financial specifics of the project.
Solar radiation Tracker has played a vital role in increasing the efficiency of solar panels in
recent years, thus proving to be a better technological achievement. The vital importance of a
dual axis solar tracker lies in its better efficiency and sustainability to give a better output
compared to a fived solar panel or a single axis solar tracker. The tracking system is designed
such that it can trap the solar energy in all possible directions. Generally, in a single axis
tracker that moves only along a single axis it is not possible to track the maximum solar
energy. In case of dual axis trackers, if the solar rays are perpendicular to panel throughout
the year. Hence, maximum possible energy is trapped throughout the day as well as
throughout the year. Thus, the output increases indicating that the efficiency more than a
fixed solar panel (about 30 -40% more) or a single axis solar tracker (about 6-7% more).
___
### __License__ ###

```
MIT License

Copyright © 2020 Divyanshu Jha

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "software"),
to deal in the Software without restriction, including without limitation the 
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
