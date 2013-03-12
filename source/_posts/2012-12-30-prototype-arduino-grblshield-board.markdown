---
title: Prototype Arduino + grblShield Board
author: Duane Johnson
layout: post
permalink: /2012/12/prototype-arduino-grblshield-board/
categories:
  - Uncategorized
tags:
  - arduino uno
  - grbl
  - grblshield
  - prototype board
  - switching bec
---
# 

A switching BEC (battery elimination circuit) arrived from HobbyKing a couple of days ago. This converts my 12V battery power supply down to 5V for the Arduino. It can convert much higher voltage (up to 40V) but I don’t think I’ll be using that for now ![:)][1] 

 [1]: http://makerslider.com/wp/wp-includes/images/smilies/icon_smile.gif

When all strapped together, the prototype board is quite a sight (ok, an ‘ugly’ sight if you ask me). It’s kind of cool to be able to put all of these pieces together, though, and get a programmable board that does exactly what’s needed: slide a camera back and forth using a stepper motor at variable speed.

[![][3]][3] 


I’m having a bit of trouble getting the potentiometer knob to make a solid connection with the Arduino. As a result, the speed control behaves somewhat “randomly” whenever it samples the potentiometer’s resistance (it’s a 10k ohm pot). I’m hoping that once soldered on a proper PCB board the variability will go away–when I physically clamp the wires together with my fingers, I get a predictable result, for example.

 []: https://www.dropbox.com/s/38w5fxuz1i5p0g5/2012-12-30-prototype-board.jpg

The source code for the modified version of grbl is available here: 

This version of grbl basically adds the ability to sample analog pin values (as is needed with the potentiometer) and uses the anolog pins for buttons as well (since all of the digital pins are used up by the grblShield’s XYZ axes).