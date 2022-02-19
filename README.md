# 128K expansion board for Timex Computers 
### limited to Portuguese models TC 2048, TC 2068 and Polish UK2086
based on [Superfo's works](https://worldofspectrum.org/forums/discussion/comment/790105/#Comment_790105)

© 2022 KWF

Date: 19/02/2022

Revision: 0.2

![3D model](/Docs/TC2068_128K_4in1_v0_2.png)

#### Embeded and tested features:

* 2 x 32KB ROM                                                (checked)
* 128 KB RAM with ZX Spectrum +2A/B & +3 paging modes         (checked)
* control logic in CPLD (XC9536XL type)                       (checked)
* AY-3-8910 sound chip controlled with ZX128K ports           (checked)
* Kempston joystick interface                                 (checked)
* RGB video outputs                                           (checked)
* RESET button                                                (checked)

If you are interested in hardware's tests and how it works, have a look there: [YouTube](https://youtu.be/7duh5zHNvDc)

The version 0.2 will be open to with schematic and Gerber files available to the publiic. The CPLD impletmentation is closed and the complie file will be available only. 

Note that any other inteface with its own ROM requires additional wiring around /ROMCS lines (towards TC2068 and incomming from any other extenal interface). The wiring enables compability with interfaces like DivMMC/DivSD however they require basic knowlage of electronic. Also the order of interfaces connected to TC2068 is cricital and the first device to the computer edge connector must be TMX128.

### Use with TC2048

The IF has been successfully tested with TC2048. In this case, RGB output does not works due to a different signal's alocations on the egde connector. Also a simple modification to TC2048 internals is essential. The missing /BE signal at the TC2048 edge connector needs to be wiried with a short wire from SCLD chip direcly. Pad number 4 on the top side of the main board is not used in any ZX Spectrum machine and it is recommenced for /BE wiring.

### Photos

Prototype board (rev. 0.1)
![Prototype](/Docs/4_in1__128K_TC2068.jpg)

### Warranty

*No Warranty of the Project. The Issuer makes no express or implied warranty of any kind whatsoever with respect to the Project.*

### License

GNU General Public License v3.0 T&C applies to this repository content.
