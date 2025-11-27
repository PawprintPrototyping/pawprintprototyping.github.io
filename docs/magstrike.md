
---

---
# Overview

The space has two computer-controlled doors in the kitchen: an outer one and an inner one.  This is so deliveries can access the kitchen, but not the whole space.  This page is about the inner door.

The inner door consists of:

Visionis VIS-3200 keypad, controller, and exit button kit.  [Vendor product page](https://www.visionistech.com/en/product/wireless-access-control-kit-vis-3200/)
Visionis VIS-ML300-LED magnetic strike.  [Vendor product page](https://www.visionistech.com/en/product/indoor-electromagnetic-lock-vis-ml300led/)
WeMos D1-Mini microcontroller.  [Vendor product page](https://www.wemos.cc/en/latest/d1/d1_mini.html)
ESPHome [Home page](https://esphome.io/)
CW-025 12V relay modules [Vendor product page](https://www.amazon.com/dp/B0BHLDW9G5)

# Theory of Operation

Opening the door:
The VIS-3200 controller turns the magstrike on and off.  It can be commanded to do so wirelessly, using the 433 MHz keypad in the kitchen or the wireless exit button in the main space.  It also has a wired connector which will open the door when the pins are shorted.  Home Assistant can command the microcontroller to do this, through a relay to protect the MCU's GPIOs.  The most common way Home Assistant will do this is when the exterior door is opened by the Fanvil keypad, because then HA will run automation to open the interior door (after a brief delay). 

Sensing the door status:
The microcontroller senses the door open/closed status.  The VIS-3200 controller is not involved, even though it has an input for it and supports forced open alarms.  There's a magnet on the door, and a magnetic sensor on the magstrike.  The magnetic sensor is a simple normally-open switch.  This is connected to a GPIO on the microcontroller, which exposes the state of the switch to Home Assistant to tell whether the door is open or not.

# Circuit Diagram

```
 D1 Mini
+-------+
|       |
|   D4  O----------(blue)----------O (relay  input) O---> +12V 
|       |                            [   RELAY    ]                      VIS-3200
|       |                          O (relay output) O                 +------------+
|   D3  O----(green)----+          |                +----(black)------O Open  +12V O-----(red)-----> +12V
|       |               |          +----------(green)-----------------O Gnd    Gnd O-----(black)---> ground 
+-------+               |                                             |            |
                 [Door sensor]               + -------------(red)-----O Lock+      |
                        |                    |              +-(black)-O Ground     |
                        v              [ MAGSTRIKE ]        |         +------------+
                     ground                  +-----------+  |
                                                         v  v
                                                        ground
```

# Users

The VIS-3200 has been programmed with two unlimited-use users, #1 and #69, which have PIN codes based on non-random numbers found in popular culture.  There are also three one-time use codes for users 020, 021, and 022 (the leading zero indicates a limited-use "guest" user), which have been distributed to the board for use in circumstances where they may need to remotely grant someone access to the space on a one-time use basis.

The VIS-3200 does have a built-in 125 kHz prox reader, but it is not used in our deployment.
