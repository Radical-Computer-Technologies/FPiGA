# FPiGA-CoreLib
Radical Computer Technologies public repository for the FPiGA CoreLib including both HDL source for the core library as well as linterfacing software libraries/drivers for the Raspberry Pi and other "Pi-like" platforms.

## Overview
FPiGA was bred out of the interest of defining a hardware and software standard for interfacing FPGAs with Raspberry Pi type platforms. To date, tbere bas not been a standardized approach to interfacing with Raspberry Pis from FPGAs. This has led to
a calvacade of different implementations. To simplify the matter and to approach this from a KISS ("keep it simple, stupid") 
approach, this project aims to develop standard hardware interfaces, standardized HDL IP libraries, standardized device 
drivers, and standardized hardware libraries to simplify development.

Core concepts of compliance:
* Maintain standard hardware interfacing
* Maintain standard kernel/bare metal drivers
* Maintain standard HDL IP Cores across various vendors
* Maintain standard user space software libraries

## Hardware Interfaces
Hardware interfaces can currently be separated into two standardized formats (CPU<->FPGA and FPGA Interfaces). 

### CFPGA Interface (CPU to/from FPGA)
These interfaces provide communication and data transfer to/from CPUs and FPGAs.

### FPGA Interface
* These Interfaces proved communication and data transfer to/from FPGAs and other hardware devices.

As this is an ambitious goal and considering we are still working within Alpha stages, we are keeping true to the KISS approach
and have started our base design using I2C as the communication interface. Further, with the first hat board made being an audio interface, we have also included

Supported CPU <-> FPGA Interfaces:
* I2C
* I2S

FPGA Interfaces:
* FPiGA 8 Pin 
* I2S

Planned CPU <-> FPGA Interfaces:
* SPI 
* SMI 
* PCIe 
* MIPI 
* USB 

Planned FPGA Interfaces:
* PMOD 
* SYGYZY 
* FMC 

## Driver Implementations

Supported Driver Interfaces:
* I2C 
* I2S 

Supported ARM OS:
* Raspberry Pi OS ARM32 & ARM64

Supported Bare Metal:
* Raspberry Pi Circle

Planned OS/BareMetal Support:
* Debian ARM32 & ARM64 
* Ubuntu ARM32 & ARM64 
* Yocto ARM32 & ARM64 
* FreeRTOS
* Zephyr
* Raspberry Pi Pico C/C++
* Raspberry Pi Pico Micropython 
* Debian x86
* Ubuntu x86
* Windows ARM32 & ARM64
* Windows x86 

Supported SoC Devices:
* Raspberry Pi (2,3,4,5,CM4,CM5,Zero,Zero2W)

Planned SoC Device Support:
* Radxa Rock3, Rock5, RockCM3, RockCM5, Rock Zero3W, X2L, X4
* Orange Pi 

## HDL Cores

Supported Vendors:
* Gowin 
* Xilinx (Planned) 

## Standard Compliant Boards

* * [Radical Computer Technologies FPiGA Audio Hat (I2C/I2S/FPiGA 8 Pin)](https://github.com/Radical-Computer-Technologies/FPiGA-Audio-Hat/tree/main)

