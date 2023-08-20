# SNES Component Video Mod PCB

A PCB that carries Pb and Pr video lines with their respective components. The Y line is not on the PCB as it is just wired directly from the multi-out port instead. This mod does not work on stock SNES Jr. or "1-Chip" consoles. Compatible stock consoles **must** contain an S-ENC chip. Sometimes the S-ENC chip is labelled as "BA6594AF" or may be a revision labelled as "S-ENC A" or "S-ENC B."

![ph1S5gp](https://github.com/joshman196/SNES-Component-Video-Mod-PCB-Private/assets/114156648/36313453-5e08-4542-a5f1-64baf943a525)

## Parts Needed

- 2x 220uF 35V Capacitors [Digikey Part](https://www.digikey.com/en/products/detail/rubycon/35ZLH220MEFC8X11-5/3563385)
- 1x 0-100 Ohm Trimmer Potentiometer [Digikey Part](https://www.digikey.com/en/products/detail/bourns-inc/TC33X-2-101E/612856)
- 4x 20 Ohm Resistors [Digikey Part](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC20R0/2617312)
- 1x SS8050 Transistor [Digikey Part](https://www.digikey.com/en/products/detail/onsemi/SS8050DBU/1047260)
- 1x 100V Diode [Digikey Part](https://www.digikey.com/en/products/detail/onsemi/1N4148TR/458811)
- 3x RCA Jacks (preferrably color coded to YPbPr connections) **OR** 1x 3.5mm TRRS (4-pole) female connector with 1x 3.5mm TRRS to YPbPr adapter

You only really need 3 RCA Jacks just to do the mod since those will carry the video output and you can use the multi-out port for the audio, but you can choose to get 5 RCA jacks instead so you can also do Left and Right Audio jacks alongside the YPbPr jacks if you prefer.

## Install Guide

1. Solder the parts to the PCB and find a suitable place inside your console to put the assembled board at so you can get a general idea of how long you want your wires to be. You may want to put kapton tape on the entire bottom side of the PCB or on the area of the main console board where you plan on setting the PCB down at. You may also choose to set it somewhere off of the main board.
2. Connect a wire from pin 7 on the back or bottom of the multi-out connector to either your "Y" RCA jack (the green one) or the "Y" pin of your 3.5mm 4-pole (TRRS) to YPbPr adapter. For the TRRS adapter, you can figure out which pin is which by checking continuity with a multimeter with the adapter plugged into the jack.
3. Connect a wire from pin 1 on the S-ENC chip to "Pr In" on the PCB.
4. Connect a wire from a 5V source on the main board to "+5V" on the PCB (will find a source of 5V later for the tutorial)
5. Connect a wire from pin 24 on the S-ENC chip to "Pb In" on the PCB.
6. Connect a wire from "Pr Out" on the PCB to either your "Pr" RCA jack (the red one) or the "Pr" pin of the TRRS YPbPr adapter.
7. Connect a wire from "Pb Out" on the PCB to either your "Pb" RCA jack (the blue one) or the "Pb" pin of the TRRS YPbPr adapter.
8. Connect a wire from "GND" on the PCB to a source of Ground on the SNES motherboard. There are some exposed ground planes near the 4 corners of the motherboard that you could use.
9. Set the trimmer potentiometer to 22 Ohms by using a screwdriver and turning the pot. You can measure the resistance (Ohms) by using a multimeter and putting one lead on pin facing the capacitor nearest it, and putting the other lead on the pin nearest the "TP" of the "TPOT" silkscreen label. 22 Ohms is just a starting point though, as results for every 2-chip SNES even with the same S-ENC chip seem to vary. You may want to try different values of resistance if the color output isn't to your liking. In my case, setting the potentiometer to 0 Ohms actually got me the best results.

## Credits

### Original Circuit Design:
- NightWolve (Nicholas Livaditis)

### Other Credits:
- thesteve
- Duo_R
- Michael Moffitt
