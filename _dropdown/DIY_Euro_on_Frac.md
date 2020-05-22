---
layout: page
title: Eurorack on +/- 15V
description: Euro modules on Frac systems
dropdown: DIY
priority: 1
---



There are some modules that work on +/- 15V so they are suitable for Frac DIY
I am going to include relevant information here about such a pursuit.

<!--more-->




## Laurie Bidulph (Elby Systems) on using +/-12V modules in +/-15V :


 The question is sometimes asked "Can I run my +/-12V module in my +/-15V system?" or "Can I run my +/-15V module in my +/-12V system?".

* The first factor to be considered is the maximum voltage rating of the components being used. In practise, this is really only of concern when installing a +/-12V module in to a +/-15V system as in the other case, the components already meet the requisite voltage specifications. The following notes are applicable to where a +/-12V module is being installed in to a +/-15V system.

- Passive components such as resistors and non-electrolytic capacitors are usually rated for much higher voltages such as 50V with resistors going up as high as 200V. This puts them well outside the danger zone of the voltages used in 3U/4U/5U modular systems.
    
- Electrolytic capacitors have a working voltage which should be higher than the power rails of the system. How the capacitor is being used in the circuit will determine what the maximum voltage is that will be applied across the capacitor and the working voltage must be higher than this and will result in the working voltage needing to be greater than 1x or 2x the power rail. In general, capacitors rated to 35V or more should work in most applications. Lower rated capacitors may need to be further verified - 16V capacitors should be fine when the capacitor is being exposed to voltages up to the power rail voltage of 15V.

- Tantalum capacitors also have a working voltage but this must be a lot higher than that set for electrolytics. When being exposed to levels up to the power rail voltage, it is a good rule of thumb that the working voltage should be at least 3x the power rail and so should, ideally, be rated to around 50V. 35V rated tantalums should be okay in most situations but if they are across the power rails, there is a higher risk of them failing - NB: Tantalums generally fail with a short-circuit and can cause a fire risk!.

- Most semiconductors are rated to in excess of 15V (typically 18V) and so there should be no real issue with these. However, it is always prudent to check the manufacturer's datasheets for IC's used in the module to ensure that they are rated for at least 15V. Some devices such as the CEM family which are specified for only +/-12V operation.

- Some modules may use a voltage regulator or similar device to generate an internal power rail such as 5V or a reference voltage. Voltage regulators will usually dissipate 'excess' voltage as heat so an increase in the power rail voltage will result in the device running hotter. It is prudent to check that the device will be running within its nominal power rating with the increased voltage.

- The next factor to be considered is output levels. Many modules will have their output levels configured to a certain output level e.g a VCO may have all its outputs swing between +/-5V. This is often set through the use of a resistive divider network. In these situations, changing from +/-12V to +/-15V would result in those output levels increasing by around 25% eg a +/-5V output increasing to +/-6.25V while changing from +/-15V to +/-12V would reduce the output levels eg +/-5V would become +/-4.0V. The user will need to determine if these changes are significant and whether adjustments are needed. This adjustment will often be simply a matter of changing the value of a resistor.

- Another factor is the use of internal reference levels that are implicitly tied to the power rail eg such as a simple resistive divider. These reference circuits are VERY dependent on the power rails and so changing the power rail levels will directly impact on these reference levels. This may not be critical or cause enough change to warrant modifying the circuit. For example, using a resistive divider in a +/-12V circuit to define a 2.0V reference level for a trigger circuit will result in that trigger level being raised to around 2.5V while the converse scenario will reduce that reference level to about 1.6V. Again, the user must determine if the consequence of these changes impacts the circuits operation to an extent that makes it unusable.



## +/-12V modules that work in +/-15V without any modification needed:


### Make Noise:

Wogglebug mk1 works on both  +/-12 +/-15 V according to a post from Tony Rolando

### 4ms:

Shuffling Clock Multiplier: works on +/-12-15v

Rotating Clock Divider: works on +/-12-15v

Noise Swash: works on +/-9-15v

Atoner: works on +/-12-15v 


### Flight of Harmony:

Choices: operates on +/-9-15V

Plague Bearer: operates on +/-9-15V

V'Amp: operates on +/-9-15V

Sound of Shadows: operates on +/-12-15v


### Synsi:

Stomper bassdrum module works on +/-12 an +/-15 V 

### MTM:

Spring reverb with the digital brick thingy works on  +/-12 +/-15 V without any issues

### Fonitronic:

PS3100 works on  +/-12 +/-15 V without any issues

---

### Blacet to Doepfer Power Connector

John Blacet had included this diagram on his site:

![BlacetDoepferConnector](https://github.com/FracModular/Blacet/raw/master/BlacetDoepPsConn.gif)

