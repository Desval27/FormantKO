
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

Most activity has been in the COM, NOISE, and LFOs modules. Scratch that....most activity has been bits and pieces all over.  I like to switch things up.

![COM Top Render](modules/13_COM/COM_top.png "COM Top Render")

## Modules

- [TEMPLATE](modules/00_T/README.md)

### Book 1

- [KEYBOARD INTERFACE](modules/01_KBI/README.md)
- [KEYBOARD DIVIDER](modules/02_KB_DIV/README.md)
- [INTERFACE RECEIVER](modules/03_INTF_RCVR/README.md)
- [POWER SUPPLY](modules/04_PSU/README.md)
- [VCO](modules/05_VCO/README.md)
- [VCF 12dB](modules/06_VCF_12/README.md)
- [VCF 24dB](modules/07_VCF_24/README.md)
- [RFM](modules/08_RFM/README.md)
- [ADSR](modules/09_ADSR/README.md)
- [DUAL VCA](modules/10_DUAL_VCA/README.md)
- [LFOs](modules/11_LFOs/README.md)
- [NOISE](modules/12_NOISE/README.md)
- [COM](modules/13_COM/README.md)

### Book 2

- [TOUCH CONTROLLER](modules/14_TOUCH_CONTROLLER/README.md)
- [NEW PITCH DETECTOR](modules/15_NPD/README.md)
- [DIGITAL KEYBOARD CONTROLLER](modules/16_DKC/README.md)
- [VCF EXTENSIONS](modules/17_VCF_EXT/README.md)
- [LFO SINE CONVERTER](modules/18_LFO_SINE/README.md)
- [NOISE DNG](modules/19_NOISE_DNG/README.md)
- [NOISE CNC](modules/20_NOISE_CNC/README.md)
- [COM EXTENSIONS](modules/21_COM_EXT/README.md)
- [RING MODULATOR](modules/22_RING_MODULATOR/README.md)
- [PHASE SHIFTER](modules/23_PHASE_SHIFTER/README.md)
- [KRIMISIZER](modules/24_KRIMISIZER/README.md)
- [DIGITAL REVERB](modules/25_DIGITAL_REVERB/README.md)
- [POWER SUPPLIES](modules/26_POWER_SUPPLIES/README.md)
- [KOV KB-GATE DISTRIBUTION](modules/27_KOV_KB_GATE_DISTRIBUTION/README.md)
- [MULTIPLE JACKS](modules/28_MULTIPLE_JACKS/README.md)
- [ADSR CONTROLLER](modules/29_ADSR_CONTROLLER/README.md)
- [VC LFOs](modules/30_VC_LFOs/README.md)
- [LF VCO](modules/31_LF_VCO/README.md)
- [DNG](modules/32_DNG/README.md)
- [ENV FOLLOWER](modules/33_ENV_FOLLOWER/README.md)
- [SAMPLE & HOLD](modules/34_SAMPLE_AND_HOLD/README.md)
- [WAVEFORM-PROCESSOR](modules/35_WAVEFORM_PROCESSOR/README.md)
- [MIXER](modules/36_MIXER/README.md)
- [TUNING](modules/37_TUNING/README.md)

## Panels

- [TEMPLATE_3U](panels/TEMPLATE_3U/README.md)
- [TEMPLATE_6U](panels/TEMPLATE_6U/README.md)

### Book 1

- [VCO](panels/VCO/README.md)
- [VCF-12](panels/VCF_12/README.md)
- [VCF-24](panels/VCF_24/README.md)
- [RFM](panels/RFM/README.md)
- [ADSR](panels/ADSR/README.md)
- [DUAL_VCA](panels/DUAL_VCA/README.md)
- [LFOs](panels/LFOs/README.md)
- [NOISE](panels/NOISE/README.md)
- [COM](panels/COM/README.md)

### Book 2

- [DNG](panels/DNG/README.md)
- [ENV-FOLLOWER](panels/ENV_FOLLOWER/README.md)
- [WAVEFORM-PROCESSOR](panels/WAVEFORM_PROCESSOR/README.md)
- [MIXER-3](panels/MIXER_3/README.md)
- [TUNING](panels/TUNING/README.md)

## System

- [BACKPLANE A](system/BACKPLANE_A/README.md)
- [TEST HARNESS](system/TEST_HARNESS/README.md)

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

* ±15V Power rails
* AC Mains Power (Lethal Risk)
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

