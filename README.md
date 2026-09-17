
# BSX Mini ModXo Modchip

There are a couple of points about this chip that I would like to make.

- The design is intended to make use of ENIG. HASL looks like trash compared to it and I would appreciate it if people would be willing to spend the money on it. It improves the whole board construction. It doesn't just add gold... which I absolutely would love to see.

- You must use epoxy Via filling, because the design uses Via-In-Pad. If you do not use it, Solder can creep down into teh vias and starve the pads. Tombstoning can occur on passives. That would be bad.

- The D0 dupont pin that is in teh BOM is SMD. It is NOT meant to be through hole. It will work as one, though. I use it because it makes the solder pad look nice and domed, instead of with a nasty pin poking through. A through hole part is on LCSC though, if you MUST have one. Meh.

- When ordering the JST SH 1.0mm 3 & 4P cables from China, you must specify them as such, "3P and 4P, 30CM, straight across, black. 

- When ordering the Dupont D0 cables, spring for the thinnest wires you can find. This will ultimately make it easier to solder to the point and will pose less of a risk of pulling a pad or damaging the board, although it is ALWAYS recommended to tape down the wire at the solder point in order to prevent stress and detachment from occuring.

This is a Pico modchip. You can run anything that will run on a pico, including the pico blink.uf2. It is my hope that more software will be developed that can make use of this platform and that what currently exists will continue to evolve. I designed them to run ModXo and PrometheOS, but the possibilities are endless. 

This is one of my babies. I worked hard to create a solid modchip that the community could rely on, and it absolutely is such.

It is important to note, however, that ModXO runs the RP2040 at 266 MHz, which is well beyond its stock clock speed. Not every RP2040 will reliably reach that frequency due to normal silicon-to-silicon variation. In my extended testing, this affected roughly 1 in 20 chips.

This is not a fault with the BSX Mini PCB itself. On affected boards, replacing the RP2040 with another chip resolved the issue. I have never shipped a non-working unit, because every Mini was tested before leaving me.

This discovery is one of the reasons I am moving the next generation of the design to the RP2350B. It may also be possible that later-production RP2040 silicon overclocks more consistently, but I have not tested enough newer chips to make that claim.


## Acknowledgements

This project would not have been possible had it not been for the existence of ModXo and PrometheOS. It was the vague community schematic/outline from Equinox that provided the roadmap for the modchips that I worked on every single day, 16 hours a day and for 6 months straight. They are one of my greatest achievements and I am deeply grateful to the scene for giving me that gift. THEY are the real experts. Software developers are magicians to me and I will always admire them.

 - [ModXo Github Repository](https://github.com/Team-Resurgent/modxo)
 - [PrometheOS Github](https://github.com/Team-Resurgent/PrometheOS-Firmware)


## Support

The BSX Mods Discord: https://discord.gg/H8pHk3VbH2

The BSX Mods OG Xbox Forum: https://forums.bsxmods.net

The BSX Mods store, where you can purchase the chips, as well as its big brother, the Nova: 
https://www.bsxmods.net
Password: number5isalive

