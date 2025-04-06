# cool-zero
Open-source design for Peltier powered cooler/condenser with closed coolant circuit

# Description and motivation

## Ideology
This design should be 'de-facto' considered public domain without any regard for copyrights. This is not a purely software project. This design is aimed to help people in time of extremely disturbing future events.

Since climate changes are rapidly and unexpectedly progressing, obtaining drinkable water will become expensive and/or hard. Conventionally for condensing vapors constant stream of coolant is needed (eg. running cold water). This design aims at providing simple and cheap way to obtain condensed vapor using only small amount of coolant and access to electricity.
Design is based on generic equipment that should be easily obtained. 

## Brief summary of operation
Peltier cells work with DC voltage, therefore precise current control is required. It is achieved by using MOSFET controlled by a microcontroller with PMW signal. Coolant with small reservoir is running constantly with two membrane pumps (fish tank type pump) in the coolant circuit. PCV pipe with coolant is put into spiral inside a glass jar/pot, using copper tape. Hot side of the peltier device is equiped with a copper rod and aluminum heat sink, together with fans (PC parts). Since Peltier device temperature eventually raises, microcontroller will use PID scheme to let hot side cool down.


# Contents

* /src - code for the microcontroller
* /mech - design of metal/mechanical elements
* /ee - electrical devices and circuitry
* /chem - chemistry
* /docs - detailed documentation of desing and use

* general_scheme.svg - schematic of operation
