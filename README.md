<div align="center">

  <h2>By Arnošt Dobrucký</h2>

  <p display="inline">
  
  <a href="https://creativecommons.org/licenses/by-nc/4.0/">
    <img src="https://licensebuttons.net/l/by-nc/4.0/88x31.png" alt="Creative Commons Attribution-NonCommercial 4.0 International License"></a> <a href="https://hackclub.com/">
    <img alt="Funded by Hack Club" src="https://img.shields.io/badge/Hack_Club-Funded-ec3750?style=for-the-badge&logo=hackclub&logoColor=ec3750"></img>
  </a>

  </p>

  <h4>A homemade 3D printer that just works.     :)</h4>
</div>

<sub>This work is licensed under a
[Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).
</sub>

# Table of contents
- [About](#about)
- [BOM (Bill of Materials)](#bom-bill-of-materials)
- [How to Build the Blueprint 3D Printer](#how-to-build-the-blueprint-3d-printer)
  - [Section 1 — Materials and Tools](#section-1--materials-and-tools)
  - [Section 2 — Frame and Base Construction](#section-2--frame-and-base-construction)
  - [Section 3 — Machining the Parts](#section-3--machining-the-parts)
  - [Section 4 — Assembly](#section-4--assembly)
  - [Section 5 — Mounting the BTT Eddy Duo and Display](#section-5--mounting-the-btt-eddy-duo-and-display)
  - [Section 6 — Klipper Installation](#section-6--klipper-installation)
  - [Section 7 — Calibration](#section-7--calibration)
- [Images / Videos](#imagesvideos)
- [Future Plans](#future-plans)
- [Warranty](#warranty)
- [TO DO](#to-do)

---

# About

The Blueprint 3D printer is a fully custom-built FDM 3D printer designed and constructed from scratch by Arnošt and his grandfather. Every structural component was hand-machined from steel with no pre-made frame or kit involved. The project took a total of 420 hours across design, fabrication, assembly, and calibration.

---

### Specifications

| Spec | Value |
| --- | --- |
| Build Volume | 175mm × 210mm × 200mm |
| Frame Material | Standard steel |
| Motion System | **Cartesian** |
| Mainboard | BTT Manta E3EZ v1.0 |
| Hotend | BIQU H2 V2S Lite |
| Nozzle Diameter | 0.4mm |
| Heated Bed | Yes 235mm × 235mm |
| Extruder Type | Direct Drive |
| Bed Leveling Probe | BTT Eddy Duo |
| Stepper Motors | 3× BIQU NEMA 17 |
| Power Supply | 24V — 300W |
| Control Board Host | BTT CB1 |
| Display | BTT TFT35 |
| Firmware | Klipper |
| Web Interface | Mainsail |
| Print Surface | Tape (e.g. Duct tape) |
| Max Hotend Temp | 250°C |
| Max Bed Temp | 80°C  |

---

### Key Features

- Fully custom steel frame — no off-the-shelf structural parts
- Klipper firmware with Mainsail web interface for remote control and monitoring
- BTT Eddy probe for automatic bed mesh compensation
- Custom-machined motor mounts, bed holder, and extruder mount
- Internal cable management with pre-drilled routing holes
- PSU and mainboard housed inside the base for a clean build
- Painted black steel finish throughout

# BOM (bill of materials)

| Item Description | SKU | Qty | Unit Price (USD) | Total (USD) |
| --- | --- | --- | --- | --- |
| [GT2 Timing Pulley 16/20 Teeth (20 teeth-Width 6mm-bore 8mm/10pcs)](https://biqu.equipment/products/10pcs-gt2-timing-pulley-20-teeth-alumium-bore-5mm-fit-for-gt2-belt-width-6mm-with-lower-price-for-3d-printer-part?variant=39564441124962) | WCL000020*10 | 1 | $7.21 | 7.21 |
| [BIQU H2 V2S Lite Extruder Complete Kit](https://biqu.equipment/products/h2-v2s-lite?variant=40121207554146) | 1060000581 | 1 | $58.06 | 58.06 |
| [GT2-6mm Open Timing Belt (Rubber Black/6MM/10m)](https://biqu.equipment/products/hot-sale-10meter-gt2-6mm-open-timing-belt-width-6mm-gt2-belt-for-3d-printer-parts?variant=12951056941154) | 3020040150*10 | 1 | $9.48 | 9.48 |
| [BIQU Nema17 c42 motor CNC stepper motor (Length 33mm)](https://biqu.equipment/products/nema17-c42-motor-cnc-stepper-motor-length-33mm-stepping-motor-1-33a-for-3d-printer-for-cnc-xyz?_pos=3&_psq=biqu+nema&_ss=e&_v=1.0) | 3010080001 | 3 | $11.80 | 35.39 |
| [BIGTREETECH Eddy Duo (Support USB or CAN)](https://biqu.equipment/products/bigtreetech-eddy?variant=41018205438050) | 1060000710 | 1 | $19.64 | 19.64 |
| [Flexible shaft Coupler 58mm (58/Black/4pcs)](https://biqu.equipment/products/3d-printer-stepper-motor-flexible-coupling-coupler-shaft-couplings-5mm-8mm-25mm-flexible-shaft-freeshipping-1?variant=13488032252002) | 3010050224*4 | 1 | $6.64 | 6.64 |
| [BIGTREETECH TFT35 SPI V2.1 Touch Screen for CB1](https://biqu.equipment/collections/lcd-screen/products/bigtreetech-tft35-spi-v2-1-touchscreen-io2can-module) | 1040000035 | 1 | $14.29 | 14.29 |
| [BIGTREETECH Manta E3EZ V1.0 + 5pcs EZ2209 + CB1 V2.2](https://biqu.equipment/products/bigtreetech-manta-e3ez-v1-0-for-ender3-ender3pro-ender5?variant=40214245081186) | 1020000405+… | 1 | $58.90 | 58.9 |
| [Wires](https://www.aliexpress.com/item/1005006801644262.html?spm=a2g0o.order_list.order_list_main.5.73a21802GiWhg9) | _____ | 4 | _____ | 13.58 |
| [T8 Lead Screw THSL-300-8D Trapezoidal Rod](https://www.aliexpress.com/item/1005003312523975.html?spm=a2g0o.order_list.order_list_main.36.73a21802GiWhg9) | _____ | 2 | $7.04 | 7.04 |
| [Meanwell PSU 350W](https://www.aliexpress.com/item/1005006092154615.html?spm=a2g0o.order_list.order_list_main.42.73a21802GiWhg9) | _____ | 1 | $40.34 | 40.34 |
| [Linear Rails](https://www.aliexpress.com/item/1005009577277063.html?spm=a2g0o.order_list.order_list_main.30.73a21802GiWhg9) | _____ | 3 | $18.81 | 56.43 |
| [Heat bed 235x235](https://www.aliexpress.com/item/1005007288279620.html?spm=a2g0o.order_list.order_list_main.11.73a21802GiWhg9) | _____ | 1 | $22.64 | 22.64 |
| Steel — from my grandpas garage | _____ | _____ | _____ | not yet defined |
| TOTAL: |  |  |  | 354.64 |

# How to Build the Blueprint 3D Printer

This guide explains how to build the custom steel-frame 3D printer from scratch. It covers everything from picking your materials to getting your first print. There is no pre-made kit for this — every part is made by hand. You will need basic metalworking skills, access to a drill and grinder, and patience.

## Section 1 — Materials and Tools

### Overview

Before you start cutting anything you need to have everything ready. This printer is built almost entirely from steel. You will also need a set of standard 3D printer electronics.

### What You Need

**Structural materials**

- Standard steel flat bar and sheet — for the base plate, Z-axis base, bed holder, motor mounts, and extruder mount
- Linear rails (1x for X-axis, 1x for Z-axis)
- Linear rods (1x for Z-axis)
- Lead screw with brass nut (for Z-axis)
- Aluminium extrusion or steel rod for frame uprights
- The display mount (needs to be 3D printed)
- The BTT eddy mount (needs to be 3D printed)

**Electronics**

- Mainboard (BTT Manta E3EZ v1.0)
- BTT CB1 v2.2 (runs Klipper on the printer)
- BTT  5pcs EZ2209 (the endstops)
- Stepper motors x3 (X, Y, Z)
- Heated bed 235×235
- BIQU H2 V2S Lite (the hotend)
- Power supply unit (PSU) — 24V 300W
- BTT Eddy probe (for bed leveling)
- BTT SPI 35 (The display)

**Consumables**

- Steel bolts, nuts, and washers in various sizes (M3, M4, M5)
- Stepper motor couplers
- GT2 belt and pulleys for X and Y axes
- Cable sleeves and cable ties
- Black spray paint

**Tools**

- Drill and drill bits (including metal drill bits)
- Angle grinder with cutting disc
- Files (flat and round)
- Steel square
- Vernier calipers
- Tap and die set (M3, M4, M5)
- Screwdrivers and hex keys
- Wire stripper and crimping tool
- Multimeter
- Computer with SSH access

## Section 2 — Frame and Base Construction

### Overview

The base is the foundation of the whole printer. If it is not flat and square everything built on top of it will have problems. Take your time here. We used standard steel throughout because it was the most rigid material after testing several options.

### Steps

1. **Cut the base plate** — Cut your main base plate from steel sheet to your chosen dimensions. The base needs to be large enough to house the PSU and mainboard inside it. Deburr all edges after cutting.
2. **Cut the Z-axis base** — Cut the smaller plate that the Z-axis frame will bolt onto. This sits on top of the main base plate.
3. **Mark and drill the mounting holes** — Place the Z-axis base on top of the main base plate and mark where the bolts need to go. Drill these holes carefully. Use a centre punch before drilling so the bit does not wander.
4. **Test fit everything** — Bolt the Z-axis base to the main base plate and check that it sits flat with no rocking. If it rocks, file down the high spots until it sits flat.
5. **Build the Z-axis frame uprights** — Cut and shape the vertical steel pieces that form the Z-axis frame. These need to be the same height and perfectly straight. Check with a square at every step. If anything is leaning or twisted, fix it before moving on.
6. **Bolt the Z-axis frame together** — Assemble the Z-axis frame and test fit it on the base. Check from multiple angles that it is straight and square. This step often requires making replacement parts — do not rush it.

## Section 3 — Machining the Parts

### Overview

Every bracket, mount, and holder in this printer is custom made from steel. None of these parts are bought. You make each one by cutting, drilling, and filing steel until it fits correctly. Measure everything twice before cutting.

### Steps

1. **Drill the linear rail mounting holes** — Mark and drill the holes for the linear rails on the Z-axis and X-axis frames. These holes must be accurate — rails that are even slightly crooked will cause binding during movement.
2. **Make the bed mounting bracket** — Cut and drill the bracket that holds the bed carriage to the Y-axis. Test fit it to the rods and adjust until it sits straight.
3. **Make the Y-axis rod mount** — Cut a custom steel piece that secures the Y-axis linear rods to the base. Measure the rod spacing carefully before cutting.
4. **Make the stepper motor mounts** — Cut one mount for each axis (X, Y, Z, and extruder). Each one is a different shape because each motor sits in a different position. Cut, file, and test fit each one before drilling the final bolt holes.
5. **Make the bed holder** — Cut the main bed holder from steel. This piece holds the heated bed flat so it needs to be as flat as possible. Check it against a flat surface and file down any high spots.
6. **Drill cable routing holes** — Plan the path for every cable in the printer before drilling. Mark each hole, drill it, and deburr it. Running cables through clean holes protects the insulation.
7. **Mount the PSU inside the base** — Cut any required opening for the PSU and bolt it inside the base. Make sure it is fixed firmly with no movement.
8. **Install the mainboard** — Bolt the mainboard into its housing using standoffs so it does not touch bare metal. Position it so all its connectors line up with the port holes you will cut next.
9. **Cut the port holes** — Mark the positions of the mainboard connectors on the outside of the base. Cut each hole carefully and file it smooth. Test fit a plug through each one before moving on.
10. **Make the extruder mount** — Cut the extruder mount from steel and shape it to hold the extruder at the correct position on the X-axis carriage. Drill and tap the bolt holes.
11. **Drill ventilation holes** — Drill ventilation holes in the areas of the base near the PSU and mainboard. These keep the electronics cool during long prints.

## Section 4 — Assembly

### Overview

Assembly is where everything comes together. Work through each axis one at a time. Test movement as you go — do not wait until everything is assembled before checking that axes move correctly.

### Steps

1. **Assemble the heated bed frame** — Bolt the bed frame together and run the heated bed wiring at the same time. Leave enough slack in the cable for the bed to move on the Y-axis.
2. **Assemble the X-axis** — Mount the linear rails, fit the carriage, and run the belt. Tension the belt until there is no slack but not so tight that it strains the motor. Test carriage travel across the full length.
3. **Assemble the Y-axis** — Fit the bed carriage onto the Y-axis rods and tension the belt. Check the full travel length. If the bed cannot reach the ends of its intended range, check the mounting geometry and adjust.
4. **Attach the extruder assembly** — Mount the extruder mount onto the X-axis carriage and bolt the extruder to it. Move the carriage to different positions and measure the nozzle height above the bed at each spot to confirm it is consistent.
5. **Mount the build plate** — Fit the heated bed onto its holder using four springs and thumb screws, one at each corner. Set each spring to roughly the same compression to give yourself a level starting point.
6. **Install the display and probe** — Mount the front display in its cutout and wire it to the mainboard. Mount the BTT Eddy probe next to the nozzle and wire it up.
7. **Connect all wiring** — Run every cable — motors, endstops, thermistors, heater cartridges — through the routing holes to the mainboard. Connect each one to the correct pin. Check every connection against your wiring diagram before powering on.
8. **Paint the frame** — Partially disassemble the frame and sand all steel surfaces. Apply thin coats of black spray paint and let each coat cure before adding the next. Reassemble after the final coat is fully dry.

## **Section 5 — Mounting the BTT Eddy Duo and Display**

**BTT Eddy Duo Mount**

1. Print the 3D model of the BTT eddy holder and mount it. The probe needs to sit at a fixed and measured distance from the nozzle — both horizontally and vertically — because this offset gets entered into the Klipper config and must be accurate.
2. Drill two mounting holes in the bracket to match the probe's bolt pattern.
3. Bolt the bracket to the X-axis carriage. Make sure it is rigid with no flex or wobble — if the probe moves during printing the bed mesh will be inaccurate.
4. Route its cable back along the X-axis carriage to the mainboard, securing it with cable ties so it does not hang loose near moving parts.
5. Measure the exact X and Y offset from the nozzle tip to the centre of the probe and write these values down. You will need them when setting up the probe in printer.cfg.

**Display Mount**

1. Choose a position on the front face of the base enclosure where the display will sit — it should be easy to see and reach while the printer is running.
2. Mark the outline of the display cutout on the steel and cut it out carefully with an angle grinder or drill and file. Cut slightly smaller than needed and file to the final size so the display fits snugly.
3. Drill the four corner bolt holes for the display mounting screws.
4. Bolt the display into the cutout from the inside. Use washers under the bolt heads so the display panel does not get cracked from overtightening.
5. Route the display cable through the nearest routing hole to the mainboard and connect it to the correct port.

## Section 6 — Klipper Installation

### Overview

Klipper is the firmware that runs the printer. It runs on the BTT CB1 and talks to the mainboard over USB. Mainsail is the web interface you use to control and monitor the printer from any browser on your network.

### Steps

1. **Flash the CB1** — Download the BTT CB1 OS image from [here](https://github.com/bigtreetech/CB1/releases) (specifically the version 2.3.4 , which works), extract it and flash it to a microSD card with Balena etcher . Insert it into the CB1, boot it up, and connect it to your network. Get the IP address and connect over SSH.
2. **Compile Klipper firmware** — On the CB1, go to the Klipper folder and run `make menuconfig`. Select the correct settings which are: STM32G0B1 with a "8KiB bootloader" "8 MHz crystal” and "USB (on PA11/PA12)”. Then run `make` to compile the firmware binary.
3. **Flash Klipper to the mainboard** — Put the mainboard into DFU mode (hold the BOOT button and push the RST at the same time). Now run `lsusb` you should see something like “STM32 in DFU mode” copy the id and run `make flash FLASH_DEVICE=<the id>`. It should flash it.
4. **Compile and Flash Klipper for the BTT eddy duo** — On the CB1, go to the Klipper folder and run `make menuconfig`. Select the correct settings for your mainboard's chip. Then run `make` to compile the firmware binary. Disconnect the BTT eddy cable. Push the boot button besides the connection pins [(More here)](https://github.com/krautech/btt-eddy-guide) and run `lsusb` and copy the id of something like “RPI Boot”  and flash it with `make flash FLASH_DEVICE=<the id>`.
5. **Download the configs** — This is the most important step. Download the Klipper configs from the Software folder and upload everything to the config tab in Mainsail and restart the firmware.
6. **Test each axis** — Use Mainsail to jog each axis and check it moves in the right direction. If a motor goes the wrong way add `dir_pin: !` in the config to invert it.
7. **Test homing** — Run a full home sequence and confirm all three axes home correctly without crashing.

## Section 7 — Calibration

### Overview

Calibration is not a one-time thing. You work through each step, print a test, measure it, adjust, and repeat. On a scratch-built printer this takes many sessions. Be patient and change only one thing at a time so you can see what each change does.

### Steps

1. **PID tune the hotend** — In Klipper run `PID_CALIBRATE HEATER=extruder TARGET=215`. Save the result with `SAVE_CONFIG`. This makes the hotend temperature stable.
2. **PID tune the heated bed** — Run `PID_CALIBRATE HEATER=heater_bed TARGET=55`. Save the result. This makes the bed temperature stable.
3. **Calibrate extruder rotation distance** — Mark 100mm of filament from the extruder entry. Command Klipper to extrude 100mm. Measure how much filament actually moved. Calculate the corrected rotation distance with this formula: `new_rotation_distance = old_rotation_distance * (actual_mm / requested_mm)`. Update the config and repeat until it is accurate.
4. **Set the z-offset** — Home the printer and use the paper test or probe method to find the exact distance between the nozzle and the bed. Save this as your z-offset. This controls how close the first layer is to the bed.
5. **Run bed mesh calibration** — Use the BTT Eddy probe to scan the bed surface and generate a mesh. Save it to the config. Klipper will use this mesh to compensate for any unevenness in the bed during printing.
6. **Print a test piece** — Print a small flat square to check the first layer and a 20mm cube to check dimensions. Measure the cube with calipers. Adjust rotation distances if the dimensions are off.
7. **Fix any issues** — Common problems and fixes:
    - *First layer not sticking* — lower the z-offset slightly
    - *Over-extrusion* — reduce the rotation distance
    - *Layer shifting* — check belt tension, increase motor current, or reduce print speed and acceleration
    - *Inconsistent extrusion* — check extruder grip tension and re-calibrate rotation distance
    - *Binding on an axis* — check rod and rail alignment, re-check belt tension
8. **Run a final mesh and save all settings** — After all issues are resolved, run a fresh bed mesh, re-confirm the z-offset, and save everything to the config. Add comments in the config file explaining what each setting does.

# Images/Videos

> CAD
> 
> 
> ![Screenshot 2026-03-22 175751.png](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/Screenshot%202026-03-22%20175751.png?raw=true)
> 
> ![Screenshot 2026-03-22 175859.png](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/Screenshot%202026-03-22%20175859.png?raw=true)
> 
> ![Screenshot 2026-03-22 175927.png](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/Screenshot%202026-03-22%20175927.png?raw=true)
> 
> ![Screenshot 2026-03-22 175943.png](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/Screenshot%202026-03-22%20175943.png?raw=true)
> 

> Printer IRL
> 
> 
> ![20260214_110800.jpg](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/20260214_110800.jpg?raw=true)
> 
> ![20260214_110807.jpg](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/20260214_110807.jpg?raw=true)
> 
> ![20260214_110838.jpg](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/20260214_110838.jpg?raw=true)
> 
> ![20260214_120433.jpg](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Photos%20&%20Videos/20260214_120433.jpg?raw=true)
> 

> video of the printer running at max acceleration
> ![]([https://github.com/Arnost55/Custom-3D-printer---blueprint/raw/refs/heads/main/Photos%20&%20Videos/Frame%20showoff.mp4](https://video-downloads.googleusercontent.com/ADGPM2mlYGiEdkS8g0pUzws98QiqXWsKTgaZ3htY1w1jN-sAJujNoViGuErOnH-SIfxhGw_FDsqDPu0a7FY5S2uDYurboXzC-bbGNi9L1O2M8MC75wNYty0Q48O6LM2Lj2oHSrB8_wHD76lJhYgHL_mLV-aKTE9YZdjeKj_r1EnzSNZ0J6Y-_NUrRx7ISIeRLmE-bxCJ5Q8ADp0jfbDlhgHAA3gvltoJDUJefFQvR23cXp3FoYIm7TnOqxPwYnYqk7XJRIjw2gyPYsnkvRmw8Ob6BlHgOulF7PehC7p1CpI9xK4mYPLu30boFTKEcKAHG4r_Tii4aKVjgieETHybsFFNwy-qggP8LtEaHbPMO5VhQyrH-vKXgZdOVIJ6CRrtYLw6AeYo6Vd6bpaBDws-SCyhmew6yGt4gBbcdP1lVyhTNsYnUuIiYq7V-EZRSXPeyHdLhaG7qYTSL5ax_bC87mDVb-Q4ZLhB34utnVuxIOqSK6MkNYndSRUaVsfW-v93DJvJJ2M8AvAgnxRSRkH7557U8nqKs4pVRGFz1SIEdWUjW5qDZCjUIIwcMmpHuKlQ_z7FiTWrnEwPco4yXzl37KmrMqqrdx95eSxiex1vkV_JK9sqFMfZkZtR7alqWJJNDACgHZXSSGE6mtlpwVqef_o94JZyAi3c7LIlDRrXpum6cUvzQgUwky_ssvZQ9IOwnGng494UVxyk8wVTrFkUXdJDW8fKsW4xDjQ8QijW-1GI6QA54EsmEASHL6XcuYGFTrJ_78cchLIEVOt3oN2nzy103fA79DrfSt9RjAeKUBmibSE4l9gbEgwU_0w7D0D7N2L6Gr9X-5hGErI2HhyJsH3GsmOIWOoH6OcnPZhKCmFu5WPUaLCeBwuGSW085oGbs1W_YjlcJuEmC79Y-MgSTH7mD4K4HFcqUFTA0ac_OAWEe-3LJ_92JNO4G5lmbrjCm5jTop8HD02-WTVIOxp_Gg1wT0PQwLgP_EJSg3egNsynznm3ym8EjG8_6g-rwRoaOAF8vZMSYx27siGDwTbeTXIzRNj8K8CdNXvz0AHK0BvoBo6nWrCdqEbzZ2uWByM9doDtgJqwHXl-FbyQZmh3fDySVloUNknIuqHQAqjDVEWgEIBrch5OpwcY0aWZxsT3Qetg3KWNY-nMS1lZQjuVufi61UovXMrn1-t9ifNoU6c4yMA3w2kjnbG7KVnmEHr-OFIOj1AaSE6-rwKUbA0QduPhpm7EFFjYtl39jiozwV104JQ-eiz7kEc?authuser=0))

## Wiring diagram

![Wiring diagram for the printer.png](https://github.com/Arnost55/Custom-3D-printer---blueprint/blob/main/Hardware/Wiring%20diagram%20for%20the%20printer.png)

Wiring diagram for the printer.png

# Future plans

This project has no future plans.

The Blueprint 3D printer was built as a one-time project specifically for the Blueprint programme. It was never intended to be a product, a kit, or a continued development effort. The goal was to design and build a fully functional 3D printer from scratch, and that goal has been completed.

No further versions are planned. No improvements, upgrades, or continuations of this project are in development. This document and the build journals represent the full and final record of the project from start to finish.

# Warranty

## ⚠️ Disclaimer

This guide is provided for informational purposes only. By following this guide you accept full responsibility for your own safety and for any outcome that results from building or using this printer.

We are not responsible for any of the following:

- Personal injury or death caused by the use of tools, machinery, electricity, or the finished printer
- Damage to property, equipment, or materials during or after the build process
- Fire, electrical faults, or overheating caused by incorrect wiring, misconfigured firmware, or faulty components
- Data loss or software damage caused by following the Klipper installation or configuration steps
- Any costs, losses, or damages that arise from errors or omissions in this guide

This printer involves working with mains-voltage power supplies, high-temperature components, and moving mechanical parts. If you are not confident working with any of these, seek help from someone who is qualified before proceeding.

This guide describes how **we** built **our specific printer**. Your build will be different. Dimensions, materials, wiring, and configuration will vary depending on the parts you use. Always verify information against the official documentation for your specific components.

**Build at your own risk.**

# TO DO

- [x]  Order Parts
- [x]  Make a high resolution 3D model, CAD
- [x]  Assemble
- [x]  Make endstops
- [x]  Install klipper
- [x]  Calibrate
- [ ]  Ship it to blueprint
- [x]  GOOD VIBES, FUN
- [x]  Publish config files
