
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


