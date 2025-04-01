---
title: Laser Cutter
---

# 80W CO₂ Blue Laser Cutter

!!! abstract inline "Tool Info"
    !!! danger ":material-certificate: Certification Required"
    !!! warning ":material-hand-back-right-outline: __Do Not Hack__"
    !!! info ":material-paw: Owner: Pawprint Prototyping"

![80W Omtech Laser Cutter](/img/80w-laser.jpg){ align=right style="width: 50%"}

# Description

_Probably the tool you're here for_.

Our Chinese laser, manufactured by Omtech, features:

* 80W output
* 600 &times; 900 mm (24" &times; 35") working surface
* A Ruida controller
* ~~Rotary axis attachment~~ needs calibrating

# Safety and Certification

!!! info "Protective Equipment"
    - :material-safety-goggles: **Safety glasses**:  Polycarbonate, acrylic, or any prescription glasses
    will offer protection from IR light.  Special laser protection eyewear is in the laser computer drawer, mostly used for maintenance.
    - **Water spray bottle**: to put out small fires.

!!! danger "Hazards"
    * Laser-cutting presents a risk of fire and burns.
    * Laser-cutting certain materials can release gases that are harmful to humans and may damage the machine.
    * The laser emits invisible infrared radiation that can damage your eyes.
    * The laser is powered by high-voltage, and presents an electrocution risk if the cabinet is open.

!!! warning "Prohibited Operations"
    * Modifying or hacking the laser cutter and its accessories without board approval.
    * Bypassing interlocks or safety features.
    * Cutting materials that may harm humans or equipment.
    
## Prohibited materials

!!! warning ""
    The following materials should _NEVER_ be placed into the laser cutter.

|Material|Reason|
|--------|------|
|polycarbonate|Melts instead of burns, releases poison gas|
|vinyl|Melts instead of burns, releases poison gas|
|polyvinyl chloride (PVC)|Melts instead of burns, releases chlorine gas|
|polyvinyl butyral (PVB)|Melts instead of burns|
|neoprene|Sublimated vapors damage the optics|
|Moleskin notebooks|Contains chlorine, releases poison gas|
|ABS|Burning ABS releases hydrogen cyanide gas|
|self-laminated or glued|Anything you laminated yourself or glued together is a fire hazard|
|low-grade plywood|Excessive bowing can cause the gantry to catch on the wood being cut|
|halogenated material|Releases halogens, which can damage humans and optics|
|epoxy|Contains halogens (fluorine, chlorine, bromine, iodine)|
|phenolic resins|Contains halogens|
|chromium|Found in letaher/vegan leather: Sublimates and damages optics|
|PTFE (Teflon)|Fluorine gas is extremely corrosive|
|beryllium oxide|You don't want *anything* to do with [beryllium](https://www.osha.gov/beryllium/health-effects)|

Take care when engraving these materials:
- Flame-retardant materials, which may contain halogens like bromide.
- Manganese
- Nickel
- Cobalt
- Copper

## Pre-flight checklist

!!! info "Before every use"
    1. Make sure that the machine and workspace are clutter-free.  **The laser cutter is not a table**.
    1. Have a plan for putting out small fires without causing damage to the machine.  A small spray bottle of tap water
      or rag for smothering is usually fine for this purpose.  Verify a fire extinguisher is easily accessible in case
      things go wrong.
    1. Check that the auxiliary systems (chiller, air and exhaust) are properly connected and functional.  The Air pump
      is internal to the machine, and controlled by software. The chiller and exhaust impeller should be plugged
      directly into the laser cutter, and should turn on when the machine is running.


## Operation checklist

!!! abstract "Operational Safety"
    1. Ensure material to be cut is safe to use. See Consumable Material Reference for details.
    1. Never leave a laser cutter unattended when running a job
    1. Take care to select appropriate power/speeds settings to avoid combustion. Always start jobs with lowest power
       if unsure.

### Basic Operation Checklist

Select an appropriate power and speed for the material you are cutting.  Here are some good starting guidelines for various materials below.  Some materials are highly variable, especially wood.  Do some test cuts and engraves to dial in the right settings.  More feeds and speeds can be found [here](https://cdn.shopifycdn.net/s/files/1/0280/0012/4993/files/Average_Parameter_Settings.pdf.pdf?v=1632564433)

!!! warning "Max power level"
    The manufacturer does not recommend surpassing 70% power for any project.  You should get desired cuts or engraving quality with no more than 50-60% max power.  Running above 70% max power constantly will shorten the lifespan of the laser tube.

#### Engraving

|Material  |  Speed  |  Power  |
|----------|---------|---------|
|Clear Acrylic| 325 mm/s | 18% |
|Wood| 200 mm/s | 19%  |
|Glass| 225 mm/s | 18% |
|Leather| 400 mm/s | 16% |
|Faux Leather| 425 mm/s | 15% |
|Tile/Stones|  145 mm/s | 18% |
|Pizza (Papa John's)| 500 mm/s | 30% |

#### Cutting

| Material    | Thickness | Speed  | Power |
|-------------|-----------|--------|-------|
| Cardboard   | 1/8"      | 100 mm/s|40%  |
| Acrylic     | 1/16"     | 25 mm/s| 18%   |
| Acrylic     | 1/8"      | 12 mm/s| 25%   |
| Acrylic     | 1/4"      | 6 mm/s | 35%   |
| Arcylic     | 1/2"      | 4 mm/s | 45%   |
| Arylic      | 3/4"      | 3 mm/s | 55%   |
| Arcylic     | 1"        | 1 mm/s | 60%   |
| Birch wood  | 1/16"     | 25 mm/s| 20%   |
| Birch wood  | 1/8"      | 12 mm/s| 25%   |
| Birch wood  | 1/4"      | 7 mm/s | 30%   |
| Birch wood  | 1/2"      | 5 mm/s | 35%   |
| Birch wood  | 3/4"      | 4 mm/s | 43%   |
| Birch wood  | 1"        | 3 mm/s | 47%   |


#### Set focal distance

Our laser has an automatic focus setting. Place the material under the Z-axis sensor, press `Fn`, and use the up/down arrow to highlight `Auto Focus` setting, and press `Enter` to set the Z-height.  This will place the focus exactly at the top of the material, and set the machine Z-height to 0.  Use this setting for engraving.  For cutting, especially thick material, you will need to adjust the Z-height to the center of the material.  However since the auto-focus sets the height of the bed to the surface, and won't let you back-drive the bed to Z < 0, you will need to place another piece of material of the same thickness before using the auto-focus, and then back-drive the bed down (3/2) × (material thickness).

!!! warning ""
    Always ensure there is material under the autofocus probe.  The probe tip size is about the size of the honeycomb cells and can cause the laser head to crash into the bed and damage the motion system. If the probe misses the bed or crashes, hit the E-stop and manually back drive the bed leveling chain before restarting the machine.  Notify a board member for help with checking mirror alignment before resuming operation.



## Post-flight checklist

!!! info "End of operation and clean-up"
    1. Power down the machine
    1. Wipe surfaces
    1. Clean debris from inside as needed with shop vac.


## Useful references

### Box generators:
* [Boxes.py](https://www.festi.info/boxes.py/index.html) - an open-source, online, parametric box generator.  Also available as an inkscape plugin or as a python library.  Incredibly featured, and an incredible repository for a multitude of useful parts, including pattern tests for calibrating etching your materials.  Great resource for making an enclosure for your electronics project.
* [Makercase](https://www.makercase.com/#/) - a simpler version of boxes.py for basic enclosures.  Not as many parameters as Boxes.py, but sometimes simplicity is the best.

### Guides:
* [Laser engraving guide](https://omtechlaser.com/blogs/news/how-to-laser-engrave-for-dummies-start-to-finish-guide)

### Local material sources:
* Wood and project boards: [Home Depot](https://www.homedepot.com/b/Lumber-Composites-Plywood/N-5yc1vZbqm7/Ntk-RelaxedMatch/Ntt-glowforge?Ntx=mode+matchpartialmax&NCNI-5)
* Acrylic: [TAP Plastics](https://www.tapplastics.com/)

# Certified Members

|Member Name | Certified By | Date           |
|------------|--------------|----------------|
|Rechner Fox | (Buying it)  | 2020-04-01     |
|Kataze Skunk| Rechner Fox  | 2021-12-15     |
|Bokeh       | Kataze Skunk | 2022-04-07     |
|Mojake      | Kataze Skunk | 2022-04-07     |
|Amp         | Kataze Skunk | 2022-04-07     |
|ket         | Kataze Skunk | 2022-04-07     |
|Tigerpaw    | Kataze Skunk | 2022-04-22     |
|BrokenWing  | Rechner Fox  | 2022-05-27     |
|Robin       | Rechner Fox  | 2022-05-27     |
|Dulse       | Rechner Fox  | 2023-05-16     |
|Geo         | Mojake       | 2023-06-13     |
|Kay         | Geo          | 2023-07-29     |
|Kilte       | Geo          | 2023-09-27     |
|Bocuma      | Kilte        | 2023-11-28     |
|Z           | Rechner      | 2024-01-23     |
|Oreo        | Rechner      | 2024-03-17     |
|Stanley     | Rechner      | 2024-03-26     |
|Earthshine  | Rechner      | 2024-03-26     |
|Oddai       | Rechner      | 2024-04-23     |
|Guru        | Rechner      | 2024-05-28     |
|Crystal     | Rechner      | 2024-06-25     |
|Dingo       | Rechner      | 2024-09-03     |
|Pawbs       | Rechner      | 2024-09-03     |
|Nano        | Rechner      | 2024-09-03     |
|Dacio       | Rechner      | 2024-09-03     |
|Hufman      | Rechner      | 2024-09-03     |
|Kathiss     | Rechner      | 2025-02-25     |
|Nohi        | Rechner      | 2025-02-25     |



# Maintenance

* [Routine Cleaning video](https://www.youtube.com/watch?v=aJEYHZ4Uurc)
  * [How to clean mirrors and focal lens - blog post](https://omtechlaser.com/blogs/news/how-to-clean-laser-mirrors-and-focal-lenses)
* [Mirror Alignment](https://omtechlaser.com/blogs/news/laser-engraver-mirror-alignment-how-to-align-a-co-laser-beam)


# Tool History

|Date | Event | Noted By |
|-----|-------|-------|
|2022-03-30 | Drained and purged water from cooler.  There is some notable residue possibly from the silicone tubing connecting the chiller.  Something to keep an eye on.| Rechner
|2022-05-26 | Cleaned optics, confirmed laser beam alignment| Kataze
|2023-05-30 | Cleaned optics, greased rails, and confirmed laser alignment. | Rechner
|2024-01-22 | Drained and purged cooler water.  We probably need to add biocide | Rechner
|2024-03-26 | Cleaned main optics | Rechner
|2024-08-03 | Clean optics, greased rails, noted significant alignment problems and apparent damage from a Z-axis head crash. | Rechner
|2024-09-12 | Re-aligned 2nd mirror in an attempt to compensate for damage from Z crash. | Geo
|2025-02-04 | Replaced Y-rails and readjusted rail alignment to mostly correct Z-axis head crash damage. | Geo
|2025-03-31 | Replaced tube!  Old tube had a crack in the envelope.  Realigned.  Flushed chiller coolant and replaced silicone tubes. Alignment on x-axis is still rather skewed across full range of motion. | Rechner
