# cool-zero-zero
Open-source design for Peltier powered cooler/condenser with closed coolant circuit

# Description and motivation

## Ideology
This design should be 'de-facto' considered public domain without any regard for copyrights. This is not a purely software project. This design is aimed to help people in time of extremely disturbing future events.

Since climate changes are rapidly and unexpectedly progressing, obtaining drinkable water will become expensive and/or hard. Conventionally for condensing vapors constant stream of coolant is needed (eg. running cold water). This design aims at providing simple and cheap way to obtain condensed vapor using only small amount of coolant and access to electricity.
Design is based on generic equipment that should be easily obtained. 

## Brief summary of operation
Peltier cells work with DC voltage, therefore precise current control is required. It is achieved by using MOSFET controlled by a microcontroller with PMW signal. Coolant with small reservoir is running constantly with two membrane pumps (fish tank type pump) in the coolant circuit. PCV pipe with coolant is put into spiral inside a glass jar/pot, using copper tape. Hot side of the peltier device is equiped with a copper rod and aluminum heat sink, together with fans (PC parts). Since Peltier device temperature eventually raises, microcontroller will use PID scheme to let hot side cool down.

## Prototypes
# v1
After some careful consideration, stainless steel parts for furniture building are cheapest and easy to obtain. In this setup, M4 bolts and nuts are used.
For plastic parts to install electronics on, *back plate of CD/DVD case can be used*:
- easy to obtain
- helps with modular design
- easy to glue/screw/melt in parts


Mechanical switches + relays for each Peltier cell. 

- only passive cooling with radiators and fans - repurpose 
- coolant circuit will include *aquarim type* two pumps
- coolant reservior -- repurposed insulated can for hot bevareges


# v2
- added 'Thermal Dissipation Circuit' with 'Thermal Dissipation Liquid' (TDL) for prototype, as an alternative to simple fan/radiator setup. This will be able to dissipate ~3kW of heat (based on experts words), therefore up to 40 peltier devices (TEC1-12705) can be coupled and 'cooling capability' would require to change coolant (e.g. propylene glycol).
- power supply seems to be a problem (currently 300W), however it is possible that many power supplies to be used together (R&D needed)
- heat exchanger _on the Peltier cell_ needs to be constructed (copper pipe fi 18 mm) together with a copper plate
- insulation at Peltier cell heat exchangers need to be addressed
  - polyurethane foam - affordable, cutable, easy to get
  - styrofoam of different kinds
  - HEAT INSULATION EXPERIMENTAL SETUP WILL BE NEEDED


# Contents

* /src - code for the microcontroller
* /mech - design of metal/mechanical elements
* /ee - electrical devices and circuitry
* /chem - chemistry
* /docs - detailed documentation of desing and use

* general_scheme.svg - schematic of operation
