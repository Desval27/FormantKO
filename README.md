
# Formant Knockoff

# WIP

A somewhat authentic (at least in spirit) knockoff of the Elektor Formant™ DIY project synthesizer.  

Components that are not easily sourcable are substitued.  Substituted components or adapater boards are noted.

[Original Book 1 PDF](https://ikiwiki.laglab.org/Modular_Beast/ElektorFormantMusicSynthesiser.pdf)

DIN 41617 connecters are replaced with DIN 41612 connectors (Type B 32-PIN).  A backplane is included
as part of the project to avoid the point-to-point backend wiring of the original.  However, the current backplane 
does not currently offer more configurability compared to the original.  It simply provides a secure connection 
and reduces wiring complexity and fragility.  

The goal for verison 2 is to make both the cards and the bus system more configurable compared to the original 
normaled path (e.g. jumpers for signal routing, etc.).

## Status

![COM Render](modules/COM/COM.png "COM Render")

## Schematics

- COM: Complete
- NOISE: Complete
- LFO: Complete
- DUAL VCA: Started
- BACKPLANE: Started
- INTERFACE RECIEVER: Mostly Complete

## PCBs

- COM: Mostly complete but unbuilt.
- NOISE: Components placed.  Routing being refactored.
- LFO: components placed.  No routing.
- DUAL VCA: Started
- BACKPLAN: Started
- INTERFACE RECEIVER: Started

