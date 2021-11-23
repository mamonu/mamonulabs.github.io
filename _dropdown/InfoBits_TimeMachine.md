---
layout: page
title: Time Machine
description: Time Machine 
dropdown: InfoBits
priority: 1
---

# BLACET TIME MACHINE


- Genuine BBD Analog Delay Line Technology for that "retro" sound.
- Delays From 10 mS to 2 Seconds!
- Bi-Phase Regeneration for Killer Flanging
- Voltage Control of Most Parameters:
  * Delay Time
  * Regeneration (Feedback)
  * Modulation Rate (40 S per cycle to 40 Hz)
  * Modulation Depth
  * Effect Depth (Cancel) 
  *Reset Input for Modulation Generator for Synchronized Effects
- Envelope Follower
- External Modulation Input.
- Modulation Mixer
- Dry/Effect Mix
- Compander Noise Reduction
- Switched Capacitor Tracking Filters for Wide Delay Range with Optimum Bandwidth
- Optimized for Audio Signals from 1V to 10V 


## SPECS

- Power Requirements: 95 mA @ +15V, 75 mA @ -15V, regulated
- Module Depth: 6.5"
- Module Size: 5.25" H X 3" W
- Delay Time Response: Exponential
- CV Range: 0-10V, (0-7.5V for Delay, -5V to +5V for Regen.)
- Audio Bandwidth: (Tracks delay time) 8 KHz to 400 Hz



## TECH NOTES

### Overloading the Time Machine Audio Input


    When the audio input is too high, the TM cuts out. Reducing the input level and waiting a few seconds 
    restores normal operation. This applies to no rev and rev A PCBs.

    This problem is caused by the limited headroom of U4, the "front end" anti alias switched cap filter, 
    which is running off +/-7.5V supplies. This results in a maximum input signal level of +/-7V 
    (with input attenuator trimpot RT4 FCW).

    The TM will happily run along with typical +/-5V signal levels, but if you introduce amplification in your 
    system prior to the TM, I would suggest keeping an eye on the levels. You can adjust RT4 to allow larger 
    input signals. For example, positioning the trimmer at mid rotation, you could use signals up to 
    about +/-14V, which is around the limit of the op amps in the rest of the system. This comes at the cost 
    of 50% attenuation through the module.

    Modules built at the factory have this trimmer set at about 70% rotation which allows +/-10V signals.
    The "cutting out" of the TM is not a typical symptom of overloading an IC, but in this case, 
    the LTC1063 disturbs the power rails and shuts down both the +7.5V and -7.5V regulators! 
    This causes the "crash" of the clock driving the filters and the MN3005, which also use the +/-7.5V supplies.
    This is annoying to say the least but can be fixed with one 1N4148 diode (Dxx, shown below). 
    
    Rev B boards include this mod.
    The diode is connected between pin 14 of U6 (anode) and the +7.5V supply (cathode/band). 
    The right hand side of R26 can be used 
    for the first connection and a PCB feedthru can be used for the +7.5V. A bit of heatshrink
    will protect from shorts.Rev B PCBs have this change incorporated into the board.


### Negative CVs into Time Machine Delay Input

    This applies to no rev versions of the PCB only. The rev A and rev B versions have this change made to the board.
    If the Delay CV mix goes more than about a volt negative, the high frequency clock will stop 
    and the delayed effect will stop working. 
    Removing the negative voltage source and cycling the power will restore normal operation.

    To fix this, locate R11 and unsolder the left side, pulling up the resistor to about a 45 degree angle.
    Clean out the vacant pad with a solder sucker and insert one end of a 1K 5% resistor. Solder that end to the pad 
    and lift up the free end to mate with the free end of R11.

    Take two 1N4148 diodes and connect one cathode to the other's anode. Connect the unattached anode to the junction 
    of the two resistors above and solder the junction.

    Place some heatshrink over the two diodes and solder the unattached cathode to the feedthru just under the "2" in
    the silkscreen "Q2". (This is common.)
