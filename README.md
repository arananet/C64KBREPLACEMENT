# C64KBREPLACEMENT

The C64 Keyboard Replacement it's a project based on the MEC64 and the Simon Inns project.

# Updates

31/12/2019: Initial release.

# License

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0
International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

# Note

This is a work in progress, several testing must be made but it should work as is. I take no responsibiltiy for any damage to any equipment that results from the use of this board. USE AT YOUR OWN RISK!

If you like the project, buy me a beer :) info@arananet.net

# Images

<img src="https://github.com/arananet/C64KBREPLACEMENT/blob/master/images/a.png?raw=true" width="500">

<img src="https://github.com/arananet/C64KBREPLACEMENT/blob/master/images/b.png?raw=true" width="500">

# Connections available

There are two types of connections, one connection is via dupont cables (20 individual cables and 1 single 2.54 pin row with 20 pins) and the other is vía a USB a connector.

# Types of keyboard

With this design you can build two kind of keyboards, one keyboard is a standard C64 keyboard valid for C64 breadbin and C64C. The second version is a USB keyboard compatible with any host that allow USB keyboards, ex. Raspberry Pi, PC, MIST, etc.

The standard keyboard, only needs the cherry MX switches so no BOM needed. Only cherry keys and the pinrows for the dupont cables.

The USB version needs a little circuit logic to translate the key stroke to a usb keyboard compatible protocol. For this design you will need a BOM (bill of materials). Find it on the next table.

# Bill of materials

| Part          | Value                   | Package                        |
| ------------- | ----------------------- | ------------------------------ |          
| IC1  		| PIC18F4550-I_PT                  | QFP80                       |
| R2     		| 10K                 | 0805                   |
| R3      		| 10K                    | 0805                           |
| R4      		| 1K                    | 0805                           |
| R5    		| 150OHM | 0805        |
| X1     		| 20MHZ                   | HC49S-TH CRYSTAL OSCILLATOR                           |
| X2      		| USB-A            | USB A HEADER               |
| C1   		| 100nf                  | 0805                       |
| C2     		| 15pf                   | 0805                          |
| C3    		| 15pf    | 0805             |
| C4   		| 470nf                 | 0805                   |
