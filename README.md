
# Formant Knockoff

# WIP

A somewhat authentic (at least in spirit) knockoff of the Elektor Formant™ DIY project synthesizer.  

Components that are not easily sourcable are substitued.  Substituted components or adapater boards are noted.

[Original Book 1 PDF](https://ikiwiki.laglab.org/Modular_Beast/ElektorFormantMusicSynthesiser.pdf)

DIN 41617 connecters are replaced with DIN 41612 connectors (Type B 32-PIN).  A backplane is included
as part of the project to avoid the point-to-point backend wiring of the original.  However, the current backplane 
does not currently offer more configurability compared to the original.  It simply provides a secure connection 
and reduces wiring complexity and fragility.  

I have opted to keep the flying wires for connecting the panel components as opposed to a separate panel mounted
"control" PCB.  Right now I'm torn between keeping the layouts and wiring as they were originally defined or 
replacing them with something like JST XH connectors for easy disconnect & replacement.  Perhaps both?

The goal for verison 2 is to make both the cards and the bus system more configurable compared to the original 
normaled path (e.g. jumpers for signal routing, etc.).

## Status

Note: This information is only as accurate as I can remember to update it.

Most activity has been in the COM, NOISE, and LFOs modules.

![COM Render](modules/COM/COM.png "COM Render")

## Modules

- [TEMPLATE](modules/TEMPLATE/STATUS.md)
- [KEYBOARD INTERFACE](modules/KBI/STATUS.md)
- [INTERFACE RECEIVER](modules/INTF_RCVR/STATUS.md)
- [POWER SUPPLY](modules/PSU/STATUS.md)
- [KEYBOARD DIVIDER](modules/KB_DIV/STATUS.md)
- [VCO](modules/VCO/STATUS.md)
- [VCF 12dB](modules/VCF_12/STATUS.md)
- [VCF 24dB](modules/VCF_24/STATUS.md)
- [RFM](modules/RFM/STATUS.md)
- [ADSR](modules/ADSR/STATUS.md)
- [DUAL VCA](modules/DUAL_VCA/STATUS.md)
- [LFOs](modules/LFOs/STATUS.md)
- [NOISE](modules/NOISE/STATUS.md)
- [COM](modules/COM/STATUS.md)

## Panels

## System

- BACKPLANE A
- [BACKPLANE B](system/BACKPLANE_B/STATUS.md)
- [TEST HARNESS](system/TEST_HARNESS/STATUS.md)

## ⚠️ Disclaimer

This project is provided **"as is"**, without warranty of any kind, express or implied,
including but not limited to the warranties of merchantability, fitness for a
particular purpose, and noninfringement.

This is a DIY electronics project intended for educational and experimental use.
Use at your own risk.

The author assumes **no responsibility or liability** for any damage, injury, or loss
resulting from the use or misuse of this design, including but not limited to:

* Damage to connected equipment (Eurorack modules, power supplies, computers, etc.)
* Incorrect assembly or wiring
* Use with incompatible voltages or signal levels
* Personal injury

### Electrical Safety

This project may interface with:

* ±12V Eurorack power rails
* External control voltages (CV)
* Digital and analog circuitry

Improper handling may result in damage or unsafe conditions.

You are responsible for:

* Verifying all connections before powering the system
* Ensuring correct polarity of power connections
* Confirming voltage ranges and signal compatibility
* Using appropriate protection circuits where necessary

### No Guarantees

Schematics, PCB layouts, and code are provided for reference only.
They may contain errors, omissions, or design flaws.

**Always review and validate the design before building or using it.**

