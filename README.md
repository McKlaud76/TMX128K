# 128K expansion board for Timex Computers 
### limited to Portuguese TC 2068 and Polish UK 2086
based on [Superfo's works](https://worldofspectrum.org/forums/discussion/comment/790105/#Comment_790105)

© 2022 KWF

Date: 20/02/2022

Revision: 0.2 

![3D model](/Docs/TC2068_128K_4in1_01.png)

#### Embeded and tested features:

* 2 x 32KB ROM (tested OK)
* 128 KB RAM with ZX Spectrum +2A/B & +3 paging modes (tested OK)
* control logic in CPLD (tested OK)
* AY-3-8910 sound chip controlled with ZX128K ports (tested OK)
* Kempston joystick interface (tested OK)
* RGB video outputs (tested OK)
* RESET button (tested OK)

The schematic diagram is available in the /Docs sub-folder.

If you are interested in hardware's tests and how it works, have a look there: [YouTube](https://youtu.be/7duh5zHNvDc)

The version 0.2 will be open with the schematic diagram and Gerber files available to the publiic. The CPLD impletmentation is closed and the pre-compilied file will be available only. 

Note that any other inteface with its own ROM requires additional wiring around /ROMCS lines (towards TC2068 and incomming from any other extenal interface). The wiring enables compability with interfaces like DivMMC/DivSD. Also the order of interfaces connected to TC2068 is cricital. The first device attached to the computer's edge connector must be TMX128 otherwise it will now work correctly.

### Use with TC2048

The IF has been successfully tested with TC2048. In this case, RGB output does not works due to different signal's alocations on the egde connector. Also a simple modification to TC2048 internals is essential. The missing /BE signal at the TC2048 edge connector needs to be wiried with a short wire from SCLD chip direcly. Pad number 4 on the top side of the main board is not used in any ZX Spectrum machine and it is recommenced for /BE wiring.

### Photos

Prototype board (rev. 0.1)
![Prototype](/Docs/TC2068_128K_4in1_02.jpg)

### Warranty

*No Warranty of the Project. The Issuer makes no express or implied warranty of any kind whatsoever with respect to the Project.*

### License

GNU General Public License v3.0 T&C applies to this repository content.
