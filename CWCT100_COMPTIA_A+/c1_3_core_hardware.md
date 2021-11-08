---
layout: default
title: Core 1 - 3 Core Hardware
parent:  CWCT CompTIA A+
nav_order: 3
---

![image](../CompTIA_A+_Prep_3_Core_Hardware.png)

---

# CompTIA A+ (220-1001) Cert Prep 3: Core Hardware
> Learn about essential hardware components, devices, and processes as you prepare to take and pass the CompTIA A+ Core 1 (220-1001) exam.

### 1. Firmware - Objective 3.5
> Given a scenario, install and configure motherboards, CPUs and

What is BIOS/UEFI?
* firmware that is burned to the chip, used to speak to the motherboard before the OS boots up
* BIOS programs are codes
* Basic input/output services (BIOS)
* M BIOS and B BIOS - Backup BIOS

What can it do?
it talks to drive, to test the assumed hardware

#### Quick Review
* BIOS programming enables interaction with motherboard before OS loads
* BIOS is stored in nonvaltile media, thus called firmware
* POST Power On Self-Test routines are built into firmware
* The System Setup System Setup (CMOS) utility is also part of the firmware

### Firmware - POST
* As soon as power-good wire receives enough voltage, the cpu starts running and the first thing it does is talk to bios and run POST, it broadcast itselfs to the motherboard and says if you can hear me check yourself out - the all do a self check test. After the POST is succcessful, it beeps.
* It checks CPU, RAM, Video, etc.

* **Beep Codes** - error message thru error codes
* **POST cards** - has two digit hexa decimal and it tells you the error

#### Quick Review
* POST runs at boot, requesting devices to self check
* POST errors manifests as specific beep codes or display (text) codes
* POST cards enebale testing of "dead" computers

### Firmware - System Set up
* **Unified Extensible Firmware Interface(UEFI)** - an upgraded BIOS, it supplanted BIOS - but its still BIOS.

System Set up - use to change the changeable part of BIOS hold `delete` or `F2 key`

#### Quick Review
* UEFI replaces traditional 16-bit BIOS in modern systems
* The System Setup enables custom information about changeable devices
* System Setup enables changes to CPU frequencies, RAM timings, BIOS passwords, boot options, and more

### Troubleshooting Firmware

Real Time Clock (RTC) -  
Read Only Memmory(ROM) -  
CMOS Battery - the last back up, if not battery, you will lose your time or the time will slow down, if the battery dies, all the system information that you updated will disappear. Just snap in a new battery.  

**Flashing the ROM updates the firmware on flash chip** Flashing means that you're going to update all the firmware on that flashchip thats on that montherboard *very dangerous* make sure you don't run out of power - good power, make sure you get a complete copy of Flash update (Bios Flash image)

#### Quick Review
* The real-time clock battery keeps system time without external power
* The System Steup allows for changes; exit without saving is an option
* Rest System Setup for defaults
* Flash the ROM chip to update firmware

### Motherboards - Form Factor
**I/O area** -

A+ exam will define 4 specific form factor

1. ATX - biggest common form factor 12 x 9.6 in, its been around for a while 20 years standard size.
2. microATX - 9.6x9.6
3. Mini ITX - smallest form factor
4. ITX - larger version of Mini ITX  

ATX is most common.
I/O shield - are standard size

#### Quick Review
* Motherboards and cases follow standardized form factores
* Common form factors: ATX, microATX, Mini-ITX
* Power supplies offer standardized connectors

### 2. Motherboards - Chipsets

Northbridge, Southbridge - designed to work together.
**Northbridge** - interacts with the CPU, the memory, high spped
**Southbridge** - handles the connection slower stuff

Over time this changes - modern CPU takes over the Northbridge function, now its just southbridge and CPU

Its the chipset that defines all of the peripherals.

#### Quick Review
* Chipsets combine functions from many single-function chips
* Early chipsets offered Northbridge and Southbridge
* Modern chipsets feature Southbridge(CPU handles Northbridge functions)
* Chipsets define RAM capacity, USB capabilities, and much more

### Touring the Motherboard

Objective Term
SATA cables - use to connect harddrives
SATA HDD connectors -
volatge regulators and capacitors - breaks voltage to different voltages, they bubble up or expand when shut.
pcie expansion slot

pcie - is a type of expansion bus which uses serial conncetions, it received data one wire then sends data one one wire
pci - before pcie
parallel vs. serial
x16
1 x
4-lane pcie

#### Quick Review
* The motherboard manual provides essential setup information
* Montherboards come with cables, standard connectors and more
* PCIe is the most common expansion bus, it offers multiple lanes

### Touring the Case
Tower Case
Screw - Standout
Cable Manaagement

#### Quick Review
* Cases offer standardized standouts for mounting various motherboard form factors
* Better cases offer cable management features
* Pick a case that has support for number and type of drives needed

### Intsalling Motherboard - Objective 1.1
>Given a scenario, install and configure motherboards, CPUs and ...

* fan connectors are either 3 or 4 pin

#### Quick Review
* Install and test CPU and RAM on motherboard before putting in case
* Install I/O shield and triple check standout positions
* Mount motherboard and connect motherbaord cables
* Use the motherboard manual if neccessary

### 3. Power Supply - Objective 3.7
> Summarize power supply types and features

### Electricity Basics

Think of voltage like water pressure
The volumetric amount of water is the same as amperage in electricity

`volts x amps = watts`

Current - the way the electricity flows
Direct current is terrible over distances, what may start as 1000v could be reduced to 500 volts over distances
Alternating current - US standard 115 volts AC, 60Hz cycles back and forth 60 times a second

Circuit tester

#### Quick Review
* Voltage = pressure; amount of flow = amperage; V * A = Watts (work)
* DC = electrons move in same direction; AC = electrons move backa nd forth
* Use circuit tester (or multimeter) to test AC from the wall outlet

### The Power Supply

ATX power connector to motherboards

**3 main types of power**
1. 12v - yellow
2. 5v - red
3. 3.3 v - orange

**ATX 12V** - more power to motherboard
**molex** - general connector, old school
**mini connector**
**SATA** - harddrives
**PCIe** - videocards

**Modular Power Supply** - much neater solution, pick and plug in which cables to use.

#### Quick Review
* Power supplies transform AC from wall outlet to DC for the computer
* Standard connectors for motherboard are 20-24 pin ATX and 4-8 pin P4
* Use Molex and SATA connectors for peripherals and drives

### Mounting the Power Supply

#### Quick Review
* Mount power supply in case with four screws
* Orient the power supply so fans draw air from the system
* Connect motherboard primary and secondary power
* Modular PSUs offer less cable clutter than non-modular PSUs

### Choosing a Power Supply

**Volts * Amps = Watts**

How much wattage will you need? it depends, how much motherboard needs? what video cards? --> not quizzed in A+
Get the wattage you need, then add a little for buffer

When its hot the wattage is lower

80 plus efficiency - real wattage

Modular vs Saudered
Saudered is more efficeint

Standard ATX size covers almost all system

#### Quick Review

* Get a PSU with a little more wattage than your system needs
* Shop for higher-efficiency power supplies
* Modular power supplies cut down on cable clutter

### Power Protection - Objective 4.5
> Explain enviornmental impacts and appropriate controls

**Spikes and Sags**

Sag - Short term voltage dip
Brownout - Intentional or unintentional drop in voltage

Spikes or Surge = Provided more voltage than needed, can destroy the system

Surge protector/suppressors - trip alert

Cheap one is just good for one time

Uninterraptable Power Supply(UPS) - UPS batteries how long they last? --> not tested in A+

#### Quick Review
* Electricity from the source is imperfect
* Use surge protect/suppressor to proteect against spikes
* Use UPS to protect against brownouts and blackbox

### Cooling your PC

Heatsink - has copper wires and fans
if system overheats then it reboots.

Bigger fans spins slower and quiter, opposite smaller fans

PWM connectors - connects fans to motherboard

#### Quick Review

* A heat sink draws heat from electrical components
* Fans blow heater air through and out of the system
* Fan speed and noise can be controlled through firmware and software

### Trobuleshooting Power Supplies

Power supplies, takes more abuse, a burning smell is the first sign.
slow death - often shutdowns

Testing power supplies

voltage drops when testing means a slow death in power supply

#### Quick Review

* Power supplies die fast with burning smell, smoke or both
* Power supplies die slowly and cause intermittent problems
* Use PSU tester or multimeter to test power supplies

### Power Protection - Objective 5.2
> Troubleshoot problems related to motherboards, RAM, CPUs and

Clear CMOS jumper - erases all system set up settigns.

#### Quick Review

* Incorrectly installed CPUs or RAM can make it seem like your PC is dead
* Install core components and test before mounting into the case
* Errors in System Setup can cause a dead PC, try clearing the CMOS jumper
* Windows offers memory diagnostic tools to help with potentially bad RAM
