# Protocol

## sd0 - Turn console on

This command indicates that a console should turn on

## sd1 - Turn console off

This command indicates that a console should turn off

## sp[0-4] - Enable console port

This command enables a console port as up to 4 consoles can be supported by TASLink with certain replay devices

## sc[1-8] - Enable controller port

This command enables a given controller port for a console. Some consoles support Multitaps, etc to get more controllers

It also takes an argument bitmap:

Bit  Description
===  ===========
0    Plugged in
1    Overread enabled
2    (Unknown)
3    (Unknown)
4    (Unknown)
5    (Unknown)
6    24 bits per controller/32 bits per controller (7 must be enabled as well)
7    16 bits per controller/32 bits per controller (6 must be enabled as well)

## s[A-D] - Custom stream command

## se - Event

This takes an argument

## r[controllerMask] - Clear controller buffer

This resets the controller buffer for the given controllerMask

## R - Reset all consoles controller buffer

This resets the controller buffer of all connected consoles

