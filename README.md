# cool-zero-zero
Open-source design for Peltier powered cooler/condenser with closed coolant circuit

# Description and motivation

## Ideology
This design should be 'de-facto' considered public domain without any regard for copyrights. This is not a purely software project. This design is aimed to help people in time of extremely disturbing future events.

Since climate changes are rapidly and unexpectedly progressing, obtaining drinkable water will become expensive and/or hard. Conventionally for condensing vapors constant stream of coolant is needed (eg. running cold water). This design aims at providing simple and cheap way to obtain condensed vapor using only small amount of coolant and access to electricity.
Design is based on generic equipment that should be easily obtained. 

## Brief summary of operation
Peltier cells work with DC voltage, therefore precise current control is required. It is achieved by using MOSFET controlled by a microcontroller with PMW signal. Coolant with small reservoir is running constantly with two membrane pumps (fish tank type pump) in the coolant circuit. PCV pipe with coolant is put into spiral inside a glass jar/pot, using copper tape. Hot side of the peltier device is equiped with a copper rod and aluminum heat sink, together with fans (PC parts). Since Peltier device temperature eventually raises, microcontroller will use PID scheme to let hot side cool down.

- added 'Thermal Dissipation Circuit' with 'Thermal Dissipation Liquid' (TDL) for prototype, as an alternative to simple fan/radiator setup. This will be able to dissipate ~3kW of heat (based on experts words), therefore up to 40 peltier devices (TEC1-12705) can be coupled and 'cooling capability' would require to change coolant (e.g. propylene glycol).
- power supply seems to be a problem (currently 300W), however it is possible that many power supplies to be used together (R&D needed)
- heat exchanger _on the Peltier cell_ needs to be constructed (copper pipe fi 18 mm) together with a copper plate
- insulation at Peltier cell heat exchangers need to be addressed
  - polyurethane foam - affordable, cutable, easy to get
  - asbestos - too problematic, but would be easy to get
  - styrofoam of different kinds
  - HEAT INSULATION EXPERIMENTAL SETUP WILL BE NEEDED


# Contents

* /src - code for the microcontroller
* /mech - design of metal/mechanical elements
* /ee - electrical devices and circuitry
* /chem - chemistry
* /docs - detailed documentation of desing and use

* general_scheme.svg - schematic of operation
