---
layout: default
title: Core 1 - 2 Microprocessing and RAM
parent:  CWCT CompTIA A+
nav_order: 2
---
## Microprocessing - Objective 3.5
> Given a scenario, install and configure motherboards, CPUs and add-on cards

### What is a CPU?

**CPU** - central processing unit
* 8 bits == byte
* machine language
* general purpose register,
* intel 8088
* **clock** kinda like the doorbell outside the *'man in a box'*
* many *'man'* or the cpu, a pipeline or a core, on modern cpu it could be 4 steps or 16 steps
* to speed up the cpu, its to hit the clock faster.

#### Quick Review
* CPU are the chips used to run programs
* Every CPU has a internal features to process commands
* Every CPU runs code based on a specific machine language
* CPUs use pipelines to optimize the processing commands

### CPU speeds and cores
* **Herz** is one time per second
* **Giga hertz** a billion times per second
* When talking about CPU speed is were taking cpu top speed
* quartz oscillator acts like a metronone and push the clock
* motherboards tops out at about 400mhz
* clock multiplying
* overclocking - pushing the system
* multiple cores
* hyperthreading - one super smart pipleine, that can handle two incoming pcs of codes at the same time,
* each core acts like its own CPU (most cores and hyperthreading)

#### Quick Review
* CPU have a clock speed, commonly measured in GHz(billion cycles/sec)
* CPU come in primarily two makes: Intel and AMD
* CPUs take a system speed and multiply it to reach the CPU speed
* Single CPUs often have multiple cores

### Caching

SRAM - faster than regular RAM, expensive, used inside the CPU
Every CPU has RAM into it
pipeline stall - when a piece of code isnt there
comes in three cache,

Level 1 64K of RAM - runs the same speed of CPU
Level 2 128K and up -
L3 Cache - base motherboard speed

Set Association - how efficient cache

AMD - beleive in big cache,
Intel - small cache thats really smart

#### Quick Review
* CPU caching works between RAM and the CPU
* CPU is built into the CPU
* It's common to have three caches in a CPU: L1, L2 and L3

### 32-Bit vs 64-Bit Processing - Objective 1.1
>Compare and contrast common operating systems

64 wires in the address bus, 64 bit processors most common today
64 bits gives more memory
x86-32 bit = 32 bit
x64 = 64 bit

No damage in installing a 32 bit that application cannot use more than 4 GB of RAM

32 bit is alive and well today

#### Quick Review
* CPUs come in 32-bit ND 64-bit versions
* 32-bit CPUs cannot address more than 4 GB of memory
* Operating systems come in both 32 and 64-bit versions
* Most 64-bit processors alse run into 32-bit mode



Exam Tip

Install correct version of software for different version of Processor

### CPU Sockets

Intel and AMD has different microarchitecture - circuit digram of CPU, photolithography, etching away layers of silicon, using caustic chemicals and creating billions of transistors

Family names, then an *'i'* model

**Intel 1151**
* Nehalem(1st Gen)
* Sandy Bridge(2nd Gen)
* Ivy Bridge(3rd Gen)
* Haswell(4th Gen)
* Broadwell(5th Gen)
* Skylake(6th Gen)
* Kaby Lake(7th Gen)
* Coffee Lake(8th Gen)

Each new generation will have diffrent sockets

take some time and research the correct CPU and sockets

PGA and LGA
* Pin Grit Array
* Land Grit Array

LGA 1151 - the number of pins and gets bigger

Intel:
LGA 1151 - mainstream socket up enthusiast
LGA 2066 - enthusiast up to high end

AMD
AM4 - neck and neck to 1151
TR4 - enthusiast up to high end

#### Quick Review
* CPU sockets are the mount where a CPU connects to the motherboard
* CPUs microarchitectures
* Many different CPUs come from a single microarchitecture
* There are specific CPU socket packages covered on the A+

### Installing a CPU - Objective 3.5
>Given a scneario, install and configure motherboards, CPUs and

>Mike is a fan of AMD

AMD montherboard needs an AMD CPU - cannot interchange
orientation notch

CPU genertes a lot of Heat to cool it we need - OEM CPU
OEM fan
Thermal Paste - pulls heat from CPU to cooling system
A fan should be really tight, pick up the motherboard using the fan check its tight fitting
now connect it to a power - usually labelled for CPU fan
RGB lights optional

#### Quick Review
* Make sure you have the right socket and speed for your motherboard
* Always use thermal paste between the CPU and the fan
* Make sure to power the fan onto your motherboard

### Liquid Cooling
1. Overclock
2. Less noisy - OEM fan designed to take on more heat, or bigger fan(slower == quieter)


#### Quick Review
* Third party fans asre often more efficient than OEM fans
* Liquid cooling uses a pump, a radiator and a cooling clock with liquid to remove heat
* Liquid cooling reduces fan noise

### RAM Technology - Objective 3.3
> Given a scenario, install RAM types
* SDRAM - synchronous data ram, that have two notches, speed is dependent on cpu, 168 pins
* DDR SDRAM - double data rate 184 pins
* DDR2 - cover, 240 pins, sets the standard, long lifespan, has offset
* DDR3 - has offset
* DDR4 - has offset, fastest ram in comptiaA+ exam

#### Quick Review
* Different motherboards support a specific RAM technology
* The technologies on the exam are DDR, DDR2, DDR3 and DDR4
* We measure RAM speeds using DDR or PC ratings
* Multiply a DDR speed by eiight to get the PC speed

### RAM Capacity
* RAM is a square
* double sided and single sided - double is more common, look at the motherboard book to make sure
* channels - dual channel memory is common, motherboard decides - make sure RAM is identical
* RAM is sold in pairs

#### Quick Review
* Every stick of RAM has a specific capacity
* RAM comes in a single or double-sided versions
* RAM uses channels which requires RAM sticks to fill the channel
* RAM should be identical capacity in the same channel

### RAM Features
* **Parity vs ECC** - Error correction RAM, parity is a little older
* parity - 1 bad / ECC - 2 bad
* Some motherboards requires ECC

**SO DIMMS**
* for laptaps, smaller size

SPD chip - allows system to query the RAM chip

#### Quick Review
* Parity and ECC RAM contain extra chips to check for RAM errors
* ECC RAM is only for motherboards that support it
* SO DIMMS are for smaller spaces
* Almost all RAM has an SPD chip that stores information about the RAM stick
* Tools like CPU-Z read SPD information

### Installing RAM
* Check motherboard book
* if not all the RAM is there re install it again, coulbe be a problem with the channel

#### Quick Review
* Use the motherboard book to make sure you're installing the right capacity and RAM speed
* Line up the notch and drop the RAM straight into the slot
* Watch when the systme boots to verify the system sees the installed RAM
* Make sure RAM is fully installed and channels are properly filled
