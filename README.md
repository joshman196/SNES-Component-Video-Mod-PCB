# SNES Component Video Mod PCB

A PCB that carries Pb and Pr video lines with their respective components. The Y line is not on the PCB as we will just wire it directly from the multi-out port instead. This mod does not work on stock SNES Jr. or "1-Chip" consoles. Compatible stock consoles **must** contain an S-ENC chip. Sometimes the S-ENC chip is alternatively labelled as "BA6594AF" or may be a revision labelled as "S-ENC A" or "S-ENC B."

![261834495-36313453-5e08-4542-a5f1-64baf943a525](https://github.com/joshman196/SNES-Component-Video-Mod-PCB/assets/114156648/6c7e596d-b4dc-4511-9955-1846878fea07)

## Parts Needed

- 2x 220uF 6.3v Capacitors [Digikey Part](https://www.digikey.com/en/products/detail/panasonic-electronic-components/ECE-A0JKA221/44725)
- 2x 75 Ohm Resistors [Digikey Part](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNF14FTD75R0/1682415)
- 2x SS8050 Transistors [Digikey Part](https://www.digikey.com/en/products/detail/onsemi/SS8050DBU/1047260)
- 2x 1N4148 Diodes [Digikey Part](https://www.digikey.com/en/products/detail/onsemi/1N4148TR/458811)
- 3x RCA Jacks (preferrably color coded to YPbPr connections) **OR** 1x 3.5mm TRRS (4-pole) female connector with 1x 3.5mm TRRS to YPbPr adapter

For RCA jacks, you only really need 3 just to do the mod since those will carry the video output and you can use the multi-out port for the audio, but you can choose to get 5 RCA jacks instead so you can also do Left and Right Audio alongside the YPbPr jacks if you prefer. This guide does not cover the installation of audio RCA jacks.

For the TRRS jack method, it's generally considered best to desolder and remove the RF modulator from the console and put the TRRS jack in its place. If you don't want to remove the RF modulator, you will have to come up with a spot to put the TRRS jack, like drilling a hole into the shell for it. Also, you can figure out which pin on the back of the jack corresponds to which YPbPr female connector by checking continuity with a multimeter with the adapter plugged into the TRRS jack. Touch one lead of the multimeter to a pin on the back of the jack and the other lead to the inside of one of the connectors to figure out which one is which. One pin on the back of the TRRS jack may be longer than the others. This one should be the Ground pin.

## Install Guide

0. Turn off and unplug your console and open it by using a 4.5mm "Gamebit" screwdriver on the 6 screws on the bottom of the console.
1. Solder the parts to the mod PCB and find a suitable place inside your console to put the assembled board at so you can get a general idea of how long you want your wires to be. You may want to stick a layer of kapton tape covering the entire bottom side of the PCB or on the area of the main console board where you plan on setting the PCB down at. You may also choose to set the PCB somewhere off of the main board.
2. Connect a wire from pin 7 on the back or bottom of the multi-out connector to either your "Y" RCA jack (the green one) or the "Y" pin of your 3.5mm 4-pole (TRRS) to YPbPr adapter.
3. Connect a wire from pin 1 on the S-ENC chip to "Pr In" on the PCB.
4. Connect a wire from a 5V source on the main board to "+5V" on the PCB.
5. Connect a wire from pin 24 on the S-ENC chip to "Pb In" on the PCB.
6. Connect a wire from "Pr Out" on the PCB to either your "Pr" RCA jack (the red one) or the "Pr" pin of the TRRS YPbPr adapter.
7. Connect a wire from "Pb Out" on the PCB to either your "Pb" RCA jack (the blue one) or the "Pb" pin of the TRRS YPbPr adapter.
8. Connect a wire from "GND" on the PCB to a source of Ground on the SNES motherboard. There are some exposed ground planes near the 4 corners of the motherboard that you could use.

## Credits (2.x)

### Original Circuit Design:
- KPackLabs

## Credits (1.x)

### Original Circuit Design:
- NightWolve (Nicholas Livaditis)

### Other Credits:
- thesteve
- Duo_R
- Michael Moffitt
