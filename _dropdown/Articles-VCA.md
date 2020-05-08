---
layout: page
title: The Humble VCA
description: The Humble VCA
dropdown: Articles
priority: 1
---



The VCA is probably the single most overlooked module in a synthesizer system. Every synthesizer has at least one, 
a few if you're lucky. They're most often used at the tail end of the synthesizer's audio chain, taking an output 
from some sound source and gating it in conjunction with an ADSR envelope generator triggered by your keyboard 
or some other thingamajig. 

Keyboard synthesizers like the Odyssey and Minimoog have these pre-wired that way. 
Because by God that's how they were meant to be used, right?
Before we get into some less-typical uses for a VCA, let's examine what these critters are.


### Anatomy of a VCA

A VCA, otherwise known by Voltage Controlled Amplifier, Voltage Controlled Attenuator, or Two-Quadrant Multiplier 
is a high-quality gain cell with a signal input, signal output, and a control input usually fed by a summing network 
that adds two or more control voltages together. 
Frequently one of the control voltages comes from a front panel knob that determines steady-state output level.

What do we mean a high-quality gain cell? Here are some characteristics of VCAs

* Audio rejection

Everybody hates rejection, but that's one of the VCA's main jobs. When the control voltage is at zero you 
don't want to hear any of your sound source bleeding through.

* No Control Voltage feedthru

The VCA should be adjusted so that none of the control voltage ends up in your audio. Otherwise that extra thumping 
won't be your excited little heart, it's unwanted envelope transients sneaking into your sound.

* Fast response

You'll want a VCA that can keep up with your fastest attack and decay times.

* Low noise

If you hear any hissing, maybe it's the audience.

* Wide dynamic range

You want a BIG difference between the softest sound you can make and the loudest..... 
otherwise, you'd stay home and mutter to yourself in the closet.

* Near-zero DC offset

For the DC coupled VCA's, you don't want the VCA introducing any DC that would throw VCO tracking off, 
for example. DC offset should be 1 millivolt or less.

* Wide, flat frequency response

Just what you'd expect of any good amplifier ... high fidelity.


That covers the basics. To these we add:


* Linear and Exponential response modes

Since the human ear responds to the acoustic power of sound on an exponential curve, having a VCA with an 
exponential response (volt/db) is a very good thing, not only for making crisp-sounding notes with linear 
envelopes but also tremolos, level shifts, panning, etc.

You can use a linear response VCA for this but you'll need to compensate by having exponential control sources. 
At the same time, having a linear response VCA is very handy for modulating control signals ... 
assuming that the modulated control is ending up at an exponential input somewhere (e.g. VCO frequency). 
Moog's design used a single VCA with a rocker switch for linear/exponential response modes. 
Wiard has a clever pot that lets the user vary between linear and exponential. 
Serge and Doepfer offer some VCA's that are linear and others that are exponential. 
Synthesis Technology offers a linear VCA only, to be used with their exponential ADSR.

Note here also that if a VCA is linear response, it may also be DC-coupled so it can modulate the magnitude of 
control signals. For example, a sequencer or sample-and-hold voltage may be modulated by a DC coupled VCA for input 
to an oscillator so its scale can be compressed and expanded by voltage control, say, from an LFO or envelope.

* Smooth? Crunchy?

What happens when the VCA is overdriven, that is, when control voltage is applied till it takes the VCA past unity gain? 
Some manufacturers add a little signal gain but keep it clean, others let the VCA go into controlled distortion.

* Fun extras

The extras could be additional control or audio inputs, input level controls to mix the audio, or output jacks of different 
kinds to connect to different outboard equipment. 

