---
title: Magstrike

# Overview

The space has two main computer-controlled doors in the kitchen: an outer one and an inner one.  This is so delivery people can deliver items into the kitchen, without being able to access the space.  This page is about the inner door.

The inner door consists of:

Visionis VIS-3200 keypad, controller, and exit button kit.  [Vendor product page](https://www.visionistech.com/en/product/wireless-access-control-kit-vis-3200/)
Visionis VIS-ML300-LED magnetic strike.  [Vendor product page](https://www.visionistech.com/en/product/indoor-electromagnetic-lock-vis-ml300led/)
WeMos D1-Mini microcontroller.  [Vendor product page](https://www.wemos.cc/en/latest/d1/d1_mini.html)
ESPHome [Home page](https://esphome.io/)
CW-025 12V relay modules [Vendor product page](https://www.amazon.com/dp/B0BHLDW9G5)

# Theory of Operation

Opening the door:
The VIS-3200 controller turns the magstrike on and off.  It can be commanded to do so wirelessly, using the 433 MHz keypad in the kitchen or the wireless exit button in the main space.  It also has a wired connector which will open the door when the pins are shorted.  The microcontroller does this when it receives an open command from Home Assistant.

Sensing the door status:
The VIS-3200 controller is not involved.  There's a magnet on the door, and a magnetic sensor on the magstrike.  The magnetic sensor is a simple normally-open switch.  This is connected to a GPIO on the microcontroller, which exposes the state of the switch to Home Assistant to tell whether the door is open or not.

# Circuit Diagram

