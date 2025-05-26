---
layout: page
title: F355
description: F355 Morphing Dual LFO
dropdown: InfoBits
priority: 1
---




![F355](https://github.com/FracModular/fracmodular.github.io/raw/master/assets/img/BlacetF355MorphingDualLFO.png)


---

The F355 is a 2FU module with two LFOs that use our unique morphing algorithm to create over 10,000 different waveforms. 
The two outputs can vary from one cycle in 12 minutes to 1000Hz, with high and low ranges available. 
The use of a 24 MHz 32-bit ARM processor means virtually no frequency drift.

The F355 has features to make it useful in both live and in the studio. The two LFOs are "locked" to each other in one of three ways, 
chosen by a panel switch:

   -  LFO1 and LFO2 have independent rates and the same waveshape and phase
   -  LFO2 has independent waveshape but the same rate and phase as LFO1
   -  LFO1 and LFO2 have the same rate/waveshape but variable phase from 0-360°
   
   
 LFO1 can be thought of as the "master" LFO as it always has independent rate, FM, and morphing. 
 Each LFO tracks 1v/Oct and all parameters are under voltage control. 
 There are two leds that vary in brightness based on output amplitude in 128 levels.

---

The F355 uses the same morphing engine as the E350 Morphing Terrarium. The transition from one stored wavetable to another is broken down into 4096 
calculated waves. There are 3 banks of waves to select from:

 - Bank A: basic waves in order of harmonic complexity (sine, triangle, saw up, saw down, 25/50/75% pulses and noise)
 - Bank B: the waves in Bank A are repeated in frequency as 1x, 2x, 3x, 4x, etc up to 8x. This allows the LFOs to have a very wide range between them if necessary or to use this as a basic audio oscillator (limited to 1khz).
 - Bank C: the 64 waves taken from Bank C of the E350 Morphing Terrarium (created by Robert Rich) to go way beyond the ordinary. Sequences of notes, arpeggiated effects, pings, swoops, and lattice phase modulation are just a few of the options contained within. In the audio range these can be harsh, noisy, and crunchy.

There are also two external inputs to either sync the LFOs or to hold ("freeze") the outputs at the current stage of the waveform.


![F355_BANK_C](https://github.com/FracModular/fracmodular.github.io/raw/master/assets/img/F355_BankC.png)

---
