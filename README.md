# klipper-config-skr-1.3-creality-cr-10s
Klipper Configuration for a SKR 1.3 Mainboard in a Creality CR-10S 3D Printer

Because of a defect, I replaced the original Mainboard of a Creality CR-10S 3D Printer with a SKR 1.3 Mainboard with TMC2209 stepper drivers. As I am using Klipper, I needed to write a configuration file to use the CR-10S.

## 2nd Z Axis

The CR-10S has a dual Z axis with two different stepper motors. The SKR 1.3 has support for 5 drivers: X, Y, Z, Extruder 0, Extruder 1

I didn't like the idea to connect two stepper motors to one driver (as Creality did on their original mainboard) and I only have one extruder, I used the second extruder driver to drive the second Z axis. This option is supported in Klipper.

So I connected the 2nd Z axis to the E1 connector on the mainboard and it worked without a flaw.

There might be some room for improvement of the configuration, but this at least works. 


## Links and used products
* Creality 3D CR-10S 
* BIGTREETECH SKR 1.3 https://github.com/bigtreetech/BIGTREETECH-SKR-V1.3
* BIGTREETECH TMC2209 v1.2 stepper drivers https://github.com/bigtreetech/BIGTREETECH-TMC2209-V1.2
* Klipper Firmware https://github.com/KevinOConnor/klipper


