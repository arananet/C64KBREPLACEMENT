# C64KBREPLACEMENT

This project allow to build a complete mechanical keyboard for the best 8bit machine ever made, the C64. It's a project based on the MEC64 and the Simon Inns documentation. This current project is a mix of those both projects, allowing to have a C64 replacement keyboard and also use a C64 as an external o internal USB hosted keyboard (connect it to a Raspberry PI, PC, MAC or MIST). I have completely made this from ground using this two projects as reference, thanksfully because they are pretty well documented. The main reason for this it's because I bought a new C64C case from Pixelwizard ( Thomas Koch) and the C64 Ultimate Elite that I bought from Gideon Zweijtzer. 

# Project references:

MEC64 - released under MIT license https://deskthority.net/viewtopic.php?f=7&t=4522&start= or https://github.com/tltx/MeC64

The plate metal design and the keycaps adapters are from the MEC64. All the credits belong to tltx and his MEC64 project.

Simon Inns - C64 Vice Front-End https://www.waitingforfriday.com/?p=470 

Simon has made an excelent reverse engineering of the C64 original keyboard, allowing to everyone to build a C64 keyboard based on this schematics (hand made). Also have made the USB controller part used on this board.

# Files

Metal plate:
You can get the design files to build the metal plate from the DOC directory or also from the original authors of the MEC64.

https://github.com/tltx/MeC64/tree/master/plate

Keycaps adapters:
You can get the design files to build the metal plate from the KEYCAPS directory or also from the original authors of the MEC64.

https://github.com/tltx/MeC64/tree/master/keycap_adapter

USB controller firmware:
The precompiled hex file required by the pic controller is available in the HEX directory or also from the original author Simon Inns

https://www.waitingforfriday.com/wp-content/uploads/2010/01/C64-Keyboard-and-Joystick-Adaptor-Hex.zip

# Note

This is a work in progress, several testing must be made but it should work as is. I take no responsibiltiy for any damage to any equipment that results from the use of this board. USE AT YOUR OWN RISK!

If you like the project, buy me a beer or a Mercedes SLR :) info@arananet.net

# Updates

31/12/2019: Initial release.

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

# License

This project is based on the CC BY-SA but part of the files also are from the MIT license. So you must respect each one.

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0
International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

# Useful links

Cherry MX switches tested on this project:

https://es.aliexpress.com/item/32834333057.html?spm=a2g0s.9042311.0.0.274263c0MlEfpp

Long dupont cables 30cm female to female:

https://es.aliexpress.com/item/32962785036.html?spm=a2g0o.productlist.0.0.59c0501d00u8MX&algo_pvid=e06c8c27-711b-4caa-acea-0dc9f25cc1ab&algo_expid=e06c8c27-711b-4caa-acea-0dc9f25cc1ab-2&btsid=483c4871-b1f0-4b3f-97c1-bf9883f7dafe&ws_ab_test=searchweb0_0,searchweb201602_10,searchweb201603_53
