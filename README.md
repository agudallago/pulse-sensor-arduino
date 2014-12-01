pulse-sensor-arduino
====================

A simple library for using the heart rate pulse sensor in an Arduino Yún board (may be used in other boards too). Reference: https://github.com/WorldFamousElectronics/PulseSensor-Amped-Leonardo

This code just declares a simple -almost completely static- class PulseSensor which needs to be constructed with the begin() function. Once done, timer0 will be configured to sample and process every 2ms the pulse sensor wave. This is done via an ISR (Interrupt Service Routine). 

This class will keep the Signal, BPM and IBI values updated and valid in order to be retrieved and used.

