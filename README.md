# STAG_Complete

## Introduction

Flashing this code on the STM32F769I-DISC1 board makes the MCU continuously collect and process sensor data.
It then sends its inference results to a connected PC via UART.


## System requirements

If using the Makefile to compile the project, GNU Embedded Toolchain for Arm is required.
If using the Makefile to flash the code on the MCU (in terminal when inside the project folder: make flash), openocd is required.


## How to use

The MCU will be active for 10 seconds and then enter standby mode.
It can be woken from that mode by pressing the blue button on the discovery board at arbitrary times.


## Additional information

The correct drivers for the application need to be added in a directory called /Drivers. The project can also be created with the .ioc file in CubeMX, which will automatically add the neccessary drivers.
The baudrate of the UART connection is 921600 and the inference result is a string with the class name.


## Contact

Please email any questions or comments to [geigerf@student.ethz.ch](geigerf@student.ethz.ch).
