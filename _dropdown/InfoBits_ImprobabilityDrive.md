---
layout: page
title: Improbability Drive
description: Improbability Drive
dropdown: InfoBits
priority: 1
---


![ID](https://github.com/FracModular/fracmodular.github.io/raw/master/assets/img/ID.jpg)

## Controls  and  Operation

- Digital  Noise  Level  and  Width  Pots,  CV  Inputs:    
  * The  internal  analog  noise  source  is  sent  to  the  “White”  output 
  * It is also processed by a window comparator to generate a type of digital noise.

- Frequency Pot,  LP/BP Switch, CV  Input: 
  * The  internal 12 dB  filter’s frequency can  be controlled by  the pot and/or the CV jack. 
  * The switch selects a low pass or band pass response.
  * The filter’s input is the output of the Mix pot.


- Mix Pot, Mix Output: 
  * The Mix pot allows mixing  white and digital noise. This mix is sent to the filter, and the filter output is sent to the Mix Out. 
  
- S/H Pot, CV Input, External Clock Input: The S/H rate can be clocked by the internal clock via the pot and/or the 
CV jack. An external clock can also be used. Plugging in an external clock will bypass the internal one.

- White Noise Output: white noise
- Digital Noise Output: digital noise
- S/H Output: Stepped voltages derived from the filtered noise mix
- Quantized Output: Stepped voltages derived from the filtered noise mix, quantized to 1V/oct steps. 
- Trimmer  RT2  Quantizer Scale  Select:  This is  set  up with  four zones  equally  spaced. 
  * From  FCCW  to CW,  you can  select: chromatic (all the notes on a keyboard), major, minor and diminished.


## SPECS

- Front Panel Size: 5.25 x 3" W 
- Module Depth: 6.1”      
- Input/Output Jacks: 3.5 mm (1/8”)
- S/H Clock Frequency Range: 40S to 180 Hz
- Filter Frequency Range: 0 to 20 KHz
- Noise Outputs:   +/-5V max
- Power:  +/-15  Vdc  @+69/-61  mA




## MOD TECH NOTES


BananaPlug wrote:

>Hi Folks,The Blacet ID2510 (fancy noise source) has a lot of blocks in its block diagram. These simple mods give you a little more access. The usual disclaimers apply: don't get in over your head, forget about your warranty, etc. Also, I made mine with banana plugs so where I've added a jack and a switch you would probably use a switching mini-jack. I used very stubby switches so they don't crowd the knobs.

* Mod #1: There's a multi-mode filter with a switch that lets you select band pass or low passed noise as an input to a sample and hold. 
    The output of the S&H feeds a quantizer and both outputs are available at the panel. Mod #1 lets you feed the S&H / quantizer with an external signal.Add the jack & SPDT switch. Wire the jack to one side of the new switch. Take the wire off the center lug of the existing switch (Filter LP/BP) and move it to the center lug of the new switch. Run a new wire between the two remaining switch lugs.

* Mod #2: That quantizer is a nice piece of work. Good Mister Blacet even provided a choice of four scales using a little trim pot on the PCB. This mod simply remotes it to the front panel.
    Remove RT2. Install a 50K linear pot on the panel. Hook up the three wires. Piece-o-cake.


> Enjoy!

