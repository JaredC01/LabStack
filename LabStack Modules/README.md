# LabStack Modules
This section of the repository contains 3D models of items that mount into LabStack *brackets* (see the [LabStack 19](https://github.com/JaredC01/LabStack/tree/main/LabStack%2019) and [LabStack Mini](https://github.com/JaredC01/LabStack/tree/main/LabStack%20Mini) sections in the directory above this one). Each module consumes a single slot in those brackets, allowing up to four modules (eight in a 19" rack) to be mounted side-by-side while requiring only 2U of height. A brief description of each item is given in the following tables:

## STLs

| **File**                                          | **Description**                                                                                        | **Hardware Required**                       |
| :------------------------------------------------ | :----------------------------------------------------------------------------------------------------- | :------------------------------------------ |
| `Module 1x JetKVM 1x Keystone 90 Degree.stl`      | Mounts a JetKVM + one keystone slot                                                                    | Two M2 x 16mm SHCS                          |
| `Module 1x JetKVM 2x Keystone.stl`                | Mounts a JetKVM + two keystone slots                                                                   | Two M2 x 16mm SHCS                          |
| `Module 1x JetKVM.stl`                            | Mounts a JetKVM                                                                                        | Two M2 x 16mm SHCS                          |
| `Module 1x JetKVM with Logo.stl`                  | Mounts a JetKVM. Has embossed logo at rack face                                                        | Two M2 x 16mm SHCS                          |
| `Module 1x Pi 1B Rev 2.0.stl`                     | Mounts one old-school Raspberry Pi 1 Model B                                                           | Two M2 screws, two M2 nuts                  |
| `Module 1x Pi 5 with Pimoroni NVMe Base.stl`      | Mounts one Pi 5 with the [Pimoroni NVMe Base](https://shop.pimoroni.com/products/nvme-base) underneath | Hardware from Pimoroni kit                  |
| `Module 1x Pi 5 with Pimoroni NVMe Base Tall.stl` | Same as above, but allows using the taller standoffs to put the Pi "higher" above the base             | Same as above                               |
| `Module 1x Pi 5 with WisdPi 5Gbps HAT.stl`        | Mounts one Pi 5 with the [WisdPi 5GbE PoE Hat](https://www.wisdpi.com/products/wp-nh5000p)             | Hardware from WisdPi kit                    |
| `Module 1x Pi with 25 SSD.stl`                    | Mounts one Pi and one 2.5" SSD (max 9mm thick) underneath. SDD's SATA ports are exposed at rack face   | Four M3 screws, four M2.5 screws + heatsets |
| `Module 1x Pi with 2x Keystone.stl`               | Mounts one Pi + two keystone slots                                                                     | Four M2.5 screws + heatsets                 |
| `Module 1x Pi with HAT.stl`                       | Mounts one Pi, has a blank panel to be modified for any HAT                                            | Four M2.5 screws + heatsets                 |
| `Module 1x WaveShare CM4-IO-BASE with HAT.stl`    | Mounts one Pi CM4 in the [WaveShare Mini Base Board](https://www.waveshare.com/wiki/CM4-IO-BASE-B)     | Hardware from WaveShare kit                 |
| `Module 2x 25 SSD.stl`                            | Mounts two 2.5" drives, with their SATA ports exposed at rack face                                     | Four M3 screws per drive                    |
| `Module 2x JetKVM.stl`                            | Mounts two JetKVM units in a single module                                                             | Four M2 x 16 SHCS                           |
| `Module 2x Keystone.stl`                          | A blanking plate with two keystone slots                                                               | None                                        |
| `Module 2x Keystone with Passthru.stl`            | A blanking plate with two keystone slots and a generic pass-through opening                            | None                                        |
| `Module 2x Pi.stl`                                | Mounts two Raspberry Pis, without additional fans (see subsection below)                               | Eight M2.5 screws, four M 2.5 heatsets      |
| `Module 3x 25 SSD.stl`                            | Mounts three 2.5" drives, with their SATA ports exposed at rack face. Maximum thickness ~9mm per drive | Four M3 screws per drive                    |
| `Module 4x Keystone.stl`                          | A blanking plate with four keystone slots                                                              | None                                        |
| `Module Blank.stl`                                | A completely blank plate. Can be modified for custom designs                                           | None                                        |
| `Module WaveShare 2.8in DSI Display.stl`          | Mounts the [WaveShare 2.8" DSI Display](https://www.waveshare.com/wiki/2.8inch_DSI_LCD)                | Liquid/gel adhesive (optional)              |

## STLs/Module 2x Pi with Fan

This module assembly mounts two Raspberry Pis (any modern Pi with a "B" footprint should fit) in a single module slot, along with blower fan(s) to increase airflow across them.

| **File**                     | **Description**                                                        |
| :--------------------------- | :--------------------------------------------------------------------- |
| `Module 2x Pi with Fan.stl`  | Main body. Includes mount points for a fan bracket (below)             |
| `4010 Axial Mount.stl`       | Mounts a single 40x10mm blower fan such that it blows air for both Pis |
| `Dual 3007 Blower Mount.stl` | Mounts one 30x7mm blower fan for each Pi                               |
| `Dual 4010 Blower Mount.stl` | Mounts one 40x10mm blower fan for each Pi                              |


## STLs/Module Radxa X4

This module assembly mounts a [Radxa X4](https://radxa.com/products/x/x4) mini-PC. Required hardware:
 - The X4 and its included heatsink/blower fan (but not the leg frame that comes attached)
 - Four M2.5 x 25mm socket-headed cap screws (SCHS)
 - One 3D printed body (top row of table below) 
 - One 3D printed spacer (see table below)
 - (Optional) Power-over-Ethernet hat

The module is assembled as a stack, listed from bottom to top here: printed body, PoE hat (if present), printed spacer, X4, heatsink/blower fan. The printed spacer should be used on the screw that is farthest from the rack face, closest to the L-shaped shelf of the printed body. Screw through the stack and into the heatsink's tapped holes.

| **File**                               | **Description**                                          |
| :------------------------------------- | :------------------------------------------------------- |
| `Module 1x Radxa X4 with Heatsink.stl` | Main body. Includes a hexagonal cutout for PoE hat's fan |
| `Radxa X4 NO PoE HAT Spacer.stl`       | Spacer to use when NOT using PoE hat                     |
| `Radxa X4 WITH PoE HAT Spacer x4.stl`  | Spacer to use when PoE hat is installed                  |

