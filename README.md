# rpi-cm-footprints
Altium footprints for the raspberry Pi Compute Modules 4 and 5, that I designed for a personal project. I am now sharing them with the greater public. The design is intended to be as accurate as possible, yet adaptable to the concrete use cases of the circuit designer. Each variant has subvariants for different standoff heights.

## CM 5
[Link to documentation](https://pip-assets.raspberrypi.com/categories/944-raspberry-pi-compute-module-5/documents/RP-008180-DS-6-cm5-datasheet.pdf?disposition=inline)

As per chapter 4 of the documentation, there are 2 generally accepted solutions for the connector selection: [Amphenol connector part number 10164227-1001A1RLF, resulting in a stacking height of 1.5 mm with no clearance underneath the CM5](https://www.amphenol-cs.com/product/101642271001a1rlf.html), and [Amphenol connector part number 10164227-1004A1RLF, resulting in a stacking height of 4.0 mm with 2.5 mm clearance underneath the CM5](https://www.amphenol-cs.com/product/101642271004a1rlf.html). The 4 mm s [SMTSO-M25-4ET stanoffs](https://www.pemnet.com/products/product-finder/smtso-m25-4et/) for the 4 mm version, since the footprint is modeled around these series of parts. The 1.5 mm standoff choice is up to the designer, and thus, the standoff mounting holes should be resized appropriately. **Important note: Any standoff choice should have an internal metric M2.5 thread, since that is what the CM5 design is based around.**

The RPi 3D designs are taken from the [official Raspberry Pi portal](https://pip.raspberrypi.com/categories/1096-design-files).
The connector and standoff 3D files are taken from the manufacturers.

## CM 4
[Link to documentation](https://pip-assets.raspberrypi.com/categories/634-raspberry-pi-compute-module-4/documents/RP-008168-DS-2-cm4-datasheet.pdf?disposition=inline)

As per chapter 3 of the documentation, there are 2 generally accepted solutions for the connector selection: [1.5mm with mating connector (clearance under CM4 0mm): DF40C-100DS-0.4v](https://www.hirose.com/product/p/CL0684-4033-4-51), and [3.0mm with mating connector (clearance under CM4 1.5mm): DF40HC(3.0)-100DS-0.4V(51)](https://www.hirose.com/product/p/CL0684-4151-0-51#). Standoff choice is up to the user, however, I recommend the [SMTSO-M25-3ET stanoffs](https://www.pemnet.com/products/product-finder/smtso-m25-3et/) for the 3 mm version, since the footprint is modeled around these series of parts. The 1.5 mm standoff choice is up to the designer, and thus, the standoff mounting holes should be resized appropriately. **Important note: Any standoff choice should have an internal metric M2.5 thread, since that is what the CM4 design is based around.**

The RPi 3D designs are taken from [Adam Alfath on GrabCad](https://grabcad.com/library/raspberry-pi-compute-module-4-cm4-1).
The connector and standoff 3D files are taken from the manufacturers.

## Design cross-compatibility
Technically speaking, one could use the connectors and standoffs of the CM4 footprint to use on the CM5. **HOWEVER**, that is **STRONGLY ADVISED AGAINST**, since the CM5 can draw more power per pin than the CM4, and thus, can damage the connector or the CM5 in the process.

# Disclaimer
The design of the CM4 footprint has been thoroughly tested. The design *should* work for the CM5, since the raw footprint did not change, as per the Appendix B of the CM5 spec sheet, and by comparing Chapter 3 of the CM4 documentation and Chapter 4 of the CM5 documentation. However, I am yet to check that on a concrete project. The only thing that actually changed were the components being used. That being said, ***the creator is not responsible for any wrong pinout or incorrect positions that might have occured during the design phase. If you notice any, please, feel free to create an issue and I will get to it ASAP***.
