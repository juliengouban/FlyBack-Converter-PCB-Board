# FlyBack-Converter-PCB-Board

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)

The FlyBack converter converts one DC voltage and another DC voltage reduced in relation to the input voltage. It enables electronic components to be supplied at their operating voltage from an AC/DC converter, for example.

The flyback converter is probably the most widely used structure in the electronics industry (LCD monitors, CRT televisions, DVD players, etc.). It's the equivalent of a Buck-Boost converter in which the inductor has been replaced by two coupled inductors acting as transformers.
The operating principle of the Flyback converter is based on storing energy in the magnetic core of a transformer during the first phase of the switching cycle, and releasing this energy to the output during the second phase. This method of transferring energy via a transformer provides not only electrical isolation, but also great flexibility in the choice of input and output voltages.


*Project duration: 2 days*


# Table of contents
- [Electronic diagram](#electronic-diagram)
- [PCB Design](#pcb-design)
  

## Electronic diagram

In this lesson, we'll be building our own FlyBack converter from the basic circuit diagram to convert a DC voltage between 8V and 32V into two DC output voltages: 8V and 12V. 

Here's our circuit diagram, which we'll detail below:

![alt text 1](picture/1.png) 

The C4, C5, and C6 on the input are used for filtration of the input supply. Whereas R3 and R5 are used for the Under voltage lockout related purposes. 
Input elements C4, C5 and C6 are used for input power filtering.
The R2 resistor is for the On time related purpose :
![alt text 1](picture/2.png) 

We have a 7-segment 4-digit display for time, temperature and humidity : 

![alt text 1](picture/at2.png) 

## PCB Design

The PCB consists of two layers, Top Layer and Bottom Layer. We've added a micro-usb connector to the top left of the PCB so that we can power the board and program the ATtiny from Arduino IDE.

We've added a 7-segment display to read the time, temperature and humidity.

The middle of the PCB shows the ATtiny 2313A in gray. In blue we have the DHT11 sensor. Finally, at the bottom of the board is the DS1307 with a button cell to power it:

Here's the top layer view of the PCB:

![alt text 1](picture/at_pcb.png) 



Here is a 3d view of the PCB:

![alt text 1](picture/pcb_2.png) 


## Arduino Factory

 * [More details on this project](https://arduinofactory.fr/carte-pcb-station-meteo/)
  






