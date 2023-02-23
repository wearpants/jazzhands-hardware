# Jazz Hands PCBs

A small multi-PCB handheld keyboard for chording style input.

## Main

The main "brains" PCB, which accepts a nice!nano controller.
It exposes connection points with Molex Pico EZMate connectors for 5 `key` PCBs, and a 3-pin Molex Pico EZMate connector for use with the `power-reset` daughterboard PCB.
An untested IMU is also on the main PCB, for future use.

## Key

A small single key PCB with Molex Pico EZMate connector, Kailh hotswap socket, and mounting holes for possible assembly. One mounting hole "wing" is breakaway, as needed.

## Power/Reset

A small daughterboard PCB that contains a reset button and power switch, allowing those two components to be placed elsewhere in a case

# Firmware

See the `wearpants/jazzhands-zmk-config` repo for firmware for the main PCB with ZMK.

# Custom Modifications

It's possible to hack the current `main` PCB to also support a digital hall-effect sensor like the [DRV5023](https://www.ti.com/product/DRV5023) for use in a handheld "switchless design" using magnets only for activation in a glove.

# Production

All three PCBs can be produced by grabbing the generated files from the Actions tab and uploading to JLC, including partial assembly for the `main` PCB using JLC's PCBA service.
