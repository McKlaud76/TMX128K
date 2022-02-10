# 128K expansion board for Timex Computers 
### Portuguese models TC 2048, TC 2068 and Polish UK2068
based on [Superfo's works](https://worldofspectrum.org/forums/discussion/comment/790105/#Comment_790105)

© 2022 KWF

Date: 10/02/2022

Revision: 0.2 (Work in progress)

![3D model](/Docs/TC2068_128K_4in1_v0_2.png)

#### Embeded features:

* 2 x 32KB ROM,
* 128 KB RAM with ZX Spectrum +2A/B & +3 paging modes,
* control logic in CPLD (XC9536XL type)
* AY-3-8910 sound chip controlled with ZX128K ports,
* Kempston joystick interface,
* RGB video outputs,
* RESET button.

If you are interested in hardware's tests and how it works, have a look there: [YouTube](https://youtu.be/7duh5zHNvDc)

The IF has been successfully tested with TC2048. In this case, RGB output does not works due to a different signal's alocation on the egde connector. Also a simple modification to TC2048 internals is essential. The missing /BE signal at the TC2048 edge connector needs to be wiried with a short wire from SCLD chip direcly. Pad number 4 on the top side of the main board is not used in any ZX Spectrum machine and it is recommenced for /BE wiring.

### Photos

Prototype board (rev. 0.1)
![Prototype](/Docs/4_in1__128K_TC2068.jpg)

### Warranty

*No Warranty of the Project. The Issuer makes no express or implied warranty of any kind whatsoever with respect to the Project.*

### License

GNU General Public License v3.0 T&C applies to this repository content.
