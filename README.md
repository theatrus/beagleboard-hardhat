BeagleBoard Hardhat
===================

![board silk](https://raw.githubusercontent.com/theatrus/beagleboard-hardhat/master/board_silk.png)

An original design for the
[original BeagleBoard](http://beagleboard.org/Products/BeagleBoard),
originally designed in 2010, but sadly never sold as the project which
required this set of industrial I/O did not pan out.

# Features

 * 24VDC power input, which also supplies the BeagleBoard
 * Two independent 4-20mA transmitters
 * Two 4-20mA inputs
 * Two 0-10V inputs
 * Two 0-10V outputs
 * Two small isolated relay outputs
 * A UART hook up to a half-duplex RS485 transceiver.

The analog circuits were enabled via a set of I2C ADCs and DACs
(12-bit). All other controls were via GPIO control from the
BeagleBoard - there is no on-board MCU.

# Design Status

Boards were made for this design, and 2 prototypes were made from the
BOM and boards. While validation was performed, it can not be
considered bug-free.

## Boards available

A limited number of boards are available. Send an e-mail to
yann@stackfoundry.com with your mailing address. US postage is free,
International will be dealt with as it happens :-)

These boards are PCB only - no components are mounted.

# Adapting this design

All I/O to the BeagleBoard is level-shifted from 1.8V to 3.3V. If this
design is used with a 3.3V I/O device, such as a RaspberryPi, the bus
transceivers can be omitted to simply the design.

## 4-20mA transmitter

The current follower in the op-amp is a simple design, but worked well
enough in practice. The design can be modified to add more protection
against faults. The component and op-amp selection was designed to
provide tight tolerances and high performance.

## Board notes

The board is large SMT technology, and uses some fine pitch
components.

The board is "upside-down", that is the "top" faces the BeagleBoard
and the "bottom" faces the user.

## BOM Notes

A number of ceramic (MLCC) Panasonic capacitors are specified - Panasonic
exited the MLCC business, so substitutes should be found from other
suppliers (such as Samsung)




