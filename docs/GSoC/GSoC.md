# Final report for GSoC'25
My GSoC Experience with Analog Devices

## Table of Contents
1. [About Me](#example)
2. [About Analog Devices](#example2)
3. [Project Overview](#third-example)
4. [Work Done](#fourth-examplehttpwwwfourthexamplecom)
5. [Important Links](#fourth-examplehttpwwwfourthexamplecom)
6. [Future Work](#fourth-examplehttpwwwfourthexamplecom)
7. [Thanks to My Mentors](#fourth-examplehttpwwwfourthexamplecom)

## About Me
My name is Marilene Andrade Garcia. I am a computer engineer from Brazil. Since finishing my degree, I have been seeking opportunities to work in the embedded development field.

I have been working with Analog Devices under a Linux Foundation project for the past two months, writing a new Linux Kernel device driver in the Industrial Input/Output subsystem for an analog-to-digital converter (ADC).

## About Analog Devices
Analog Devices, Inc. (ADI) is an American multinational semiconductor company specializing in data conversion, signal processing, and power management technologies.

## Project Overview
When I applied for the program, the initial goal of the project was to provide support for ADE9113 chips. However, since two mentees were accepted, my mentors decided to adjust the scope and assign one device to each mentee.

I was assigned the task of providing support for the __MAX14001/MAX14002__, configurable, isolated 10-bit ADCs for multi-range binary inputs.

In addition to ADC readings, the MAX14001/MAX14002 offers several features, such as a binary comparator, filtered readings that can provide the average of the last 2, 4, or 8 ADC values, and an inrush comparator that detects inrush current. There is also a fault detection feature capable of diagnosing seven possible fault conditions, as well as an option to select either an external or internal ADC voltage reference.

## Work Done
### Assembling the Hardware Setup
- To develop and test the code, my mentors sent me a Raspberry Pi 5 and an evaluation board (MAX14001PMB), which contains two MAX14001 devices: one for measuring voltage and the other for measuring current.
- I used a USB-to-Serial FTDI232 adapter to access the Raspberry Pi terminal from my computer.
- I also configured my VLAN to allow access to the Raspberry Pi via Wi-Fi and SSH.
- Since I do not yet have a DC source, I used the Raspberry Pi’s 5V power supply and a 10K potentiometer to test voltage measurements. Unfortunately, the current supply was too low, so the current measurements were unreliable.
- I connected the MAX14001PMB with the Raspberry Pi in the following configuration.
![demo](https://github.com/MarileneGarcia/marilene.github.io/blob/main/midia/GSoC/demo.gif)


## Important Links

## Future Work

## Thanks to My Mentors