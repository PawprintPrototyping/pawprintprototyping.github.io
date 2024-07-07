---
title: EPSON Color Printer + Scanner
---

# EPSON EcoTank ET-3850 Color Printer and Scanner

!!! tldr inline "Tool Info"
    !!! warning ":material-hand-back-right-outline: __Do Not Hack__"
    !!! info ":material-paw: Owner: Pawprint Prototyping"

![EPSON ET-3850](/img/epson_et-3850.jpg){ align=right style="width: 50%" }

# Description

A wireless colo(u)r printer and scanner. It prints things, in 2D, on paper, with color.
It can be used to print stickers. It also can scan things through the top,
either through a feed or a scanner bay.

We currently use EPSON 502 BK/C/M/Y inks.

**Quick Start/Installation Guide:**
https://files.support.epson.com/docid/cpd6/cpd60031.pdf \[[Internet Archive Mirror](https://web.archive.org/web/20231127084258/https://files.support.epson.com/docid/cpd6/cpd60031.pdf)\]

**User Guide:**
https://files.support.epson.com/docid/cpd6/cpd60203.pdf \[[Internet Archive Mirror](https://web.archive.org/web/20240220130545/https://files.support.epson.com/docid/cpd6/cpd60203.pdf)\]

## Wireless Printing

When the printer is on, it usually auto-connects to the Pawprint Prototyping wifi, and
any other computers on the wifi should be able to automatically see the printer.

You can check that the printer is handling connections correctly through HTTP server.
Usually it has IP address `10.13.37.110`, but if this ever changes it can be found again
by going to `Settings (Cog icon) > General Settings > Networking Settings`.

Do note that the printer only serves HTTP and not HTTPS, so connecting to it via your
browser may give a security warning.

## Scanning

Scanning is most easily done by scanning to a memory device (USB drive). This can be
selected from the home screen option. You can also scan using a direct USB connection
with a computer.

# Safety and Certification

No certifications are required to scan or print. Don't touch wet ink and spread it around the shop.
The ink can take a bit to dry, and sometimes may never dry without additional coating or lamination.

## Hazards

!!! danger

    Printers may cause a loss of sanity.

## Printing Operation Checklist

1. Make sure the printer is on. The power button should glow white.
1. Make sure there's enough ink. The ink levels are visible on the bottom right of the printer.
1. Check that the right type of paper is loaded into the tray. The print side is **FACE DOWN**.
   The pages are loaded in from the **TOP** of the feeder.
1. Align the feeder page edge guides correctly for the page size; don't press them too tightly.
1. Check that the printer is set to the right page type. Glossy tends to make the printer move
   slower, so keep that in mind. Here's a table of known paper type combinations that we've tested.
   
   |Paper Type|Setting|Additional Notes|
   |----------|-------|----------------|
   |Standard printer paper (US Letter)| `Standard paper`|Reds may be dull|
   |JOYEZA Premium Glossy Vinyl Sticker Paper| `Premium Glossy`|Colors are good; ink rubs off really easily without additional finnishing|
   |QYH Matte Printable vinyl Sticker Paper|`Premium Matte`|Reds may be dull|
   |Printable Holographic Vinyl Sticker Paper|`Glossy`|Colors are great; ink rubs off|

1. You may now print from your standard application interface.

# Maintenance

## Refilling Ink

See the installation guide above for visual instructions.

Refilling ink can be done through the flap on the
top right of the printer, underneath the scanner unit.
Lift up the scanner unit and open up the cap for the ink
type you wish to refill.
Do NOT shake or squeeze the ink bottles. The ink will stop flowing once
the maximum ink level has been reached.

# Tool History

|Date | Event |
|-----|-------|
|||
