---
title: EPSON Color Printer + Scanner
---

# EPSON EcoTank ET-3850 Color Printer and Scanner

!!! abstract inline "Tool Info"
    !!! warning ":material-hand-back-right-outline: __Do Not Hack__"
    !!! info ":material-paw: Owner: Pawprint Prototyping"

![EPSON ET-3850](/img/epson_et-3850.jpg){ align=right style="width: 50%" }

# Description

A wireless colo(u)r printer and scanner. It prints things, in 2D, on paper, with color.
It can be used to print stickers. It also can scan things through the top,
either through a feed or a scanner bay.

We currently use EPSON 502 BK/C/M/Y inks.

* [Quick Start/Installation Guide](https://files.support.epson.com/docid/cpd6/cpd60031.pdf) \[[Internet Archive Mirror](https://web.archive.org/web/20231127084258/https://files.support.epson.com/docid/cpd6/cpd60031.pdf)\]

* [User Guide](https://files.support.epson.com/docid/cpd6/cpd60203.pdf) \[[Internet Archive Mirror](https://web.archive.org/web/20240220130545/https://files.support.epson.com/docid/cpd6/cpd60203.pdf)\]

## Wireless Printing

When the printer is on, it usually auto-connects to the Pawprint Prototyping wifi, and
any other computers on the wifi should be able to automatically see the printer.

You can check that the printer is handling connections correctly through HTTP server.
Usually it has IP address `10.13.37.110`, but if this ever changes it can be found again
by going to `Settings (Cog icon) > General Settings > Networking Settings`.

Do note that the printer only serves HTTP and not HTTPS, so connecting to it via your
browser may give a security warning.

## Scanning

Scanning is most easily done by downloading the EPSON scanning driver, which can
be downloaded here:

* [General Download link (Windows, MacOS, etc.)](https://epson.com/Support/Printers/All-In-Ones/ET-Series/Epson-ET-3850/s/SPT_C11CJ61201)
* [Linux (EPSON Scan 2)](http://download.ebz.epson.net/dsc/du/02/DriverDownloadInfo.do?LG2=EN&CN2=&DSCMI=160076&DSCCHK=3ad820ccdea5a7409e7df1603e0a16414b60a0f5)
* [Android (Google Play Store)](https://play.google.com/store/apps/details?id=com.epson.epsonsmart&hl=en_US&pli=1)
* [iOS](https://apps.apple.com/us/app/epson-smart-panel/id1477796092)

Scanning is supported over the wifi. You may need to plug in the printer IP address
into the driver to get a working connection, as detecting the printer automatically may fail.

# Safety and Certification

No certifications are required to scan or print. Don't touch wet ink and spread it around the shop.
The ink can take a bit to dry, and sometimes may never dry without additional coating or lamination.

## Hazards

!!! danger

    Printers may cause a loss of sanity.

## Printing Operation Checklist

!!! Note

    Instead of printing from Silhouette Studio, use it to export a PDF and print from
    your PDF reader of choice.  Silhouette Studio will destroy your colors if you print directly
    from it.

1. Make sure the printer is on. The power button should glow white.
1. Make sure there's enough ink. The ink levels are visible on the bottom right of the printer.
1. Check that the right type of paper is loaded into the tray. The print side is **FACE DOWN**.
   The pages are loaded in from the **TOP** of the feeder.
1. Align the feeder page edge guides correctly for the page size; don't press them too tightly.
1. Check that the printer is set to the right page type. Glossy tends to make the printer move
   slower, so keep that in mind. Here's a table of known paper type combinations that we've tested.
1. You may now print from your standard application interface.
   
   |Paper Type|Setting|Additional Notes|
   |----------|-------|----------------|
   |Standard printer paper (US Letter)|`Standard paper`|Reds may be dull|
   |JOYEZA Premium Glossy Vinyl Sticker Paper|`Premium Glossy`|Colors are good; ink rubs off really easily without additional finishing|
   |QYH Matte Printable Vinyl Sticker Paper|`Premium Matte`|Reds may be dull|
   |Printable Holographic Vinyl Sticker Paper|`Glossy`|Colors are great; ink rubs off|


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
