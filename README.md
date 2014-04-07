BeagleBoard Hardhat
===================

An original design for the
[original BeagleBoard](http://beagleboard.org/Products/BeagleBoard),
originally designed in 2010, but sadly never sold.

== Features ==

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


