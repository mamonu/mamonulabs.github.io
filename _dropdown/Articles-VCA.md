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

---

<br> 

### Anatomy of a VCA

A VCA, otherwise known by Voltage Controlled Amplifier, Voltage Controlled Attenuator, or Two-Quadrant Multiplier 
is a high-quality gain cell with a signal input, signal output, and a control input usually fed by a summing network 
that adds two or more control voltages together. 
Frequently one of the control voltages comes from a front panel knob that determines steady-state output level.

What do we mean a high-quality gain cell? Here are some characteristics of VCAs

<br> 

<br> 

##### Audio rejection

<br> 

  Everybody hates rejection, but that's one of the VCA's main jobs. When the control voltage is at zero you 
don't want to hear any of your sound source bleeding through.

<br> 

##### No Control Voltage feedthru

<br> 

  The VCA should be adjusted so that none of the control voltage ends up in your audio. Otherwise that extra thumping 
won't be your excited little heart, it's unwanted envelope transients sneaking into your sound.

<br> 

##### Fast response

<br> 

You'll want a VCA that can keep up with your fastest attack and decay times.

<br> 

##### Low noise

<br> 

  If you hear any hissing, maybe it's the audience.
  
  <br> 

##### Wide dynamic range

<br> 

  You want a BIG difference between the softest sound you can make and the loudest..... 
otherwise, you'd stay home and mutter to yourself in the closet.

<br> 

##### Near-zero DC offset

<br> 

  For the DC coupled VCA's, you don't want the VCA introducing any DC that would throw VCO tracking off, 
for example. DC offset should be 1 millivolt or less.

<br> 

##### Wide, flat frequency response

<br> 

Just what you'd expect of any good amplifier ... high fidelity.
<br> 

---


### Extras
<br> 

That covers the basics. To these we add:  

<br> 


##### Linear and Exponential response modes
<br> 

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

<br> 

##### Smooth? Crunchy?
<br> 
  What happens when the VCA is overdriven, that is, when control voltage is applied till it takes the VCA past unity gain? 
Some manufacturers add a little signal gain but keep it clean, others let the VCA go into controlled distortion.

<br> 

##### Other fun extras

<br> 

  The extras could be additional control or audio inputs, input level controls to mix the audio, or output jacks of different 
kinds to connect to different outboard equipment. 

<br> 


### VCA Trickery


As we said before, the main use most VCA's see is to gate notes with an envelope generator.
Here are a few other ideas to add to your synth arsenal:

##### Crossfading and panning

Two VCA's can be connected such that one responds to a control voltage directly and the second VCA responds inversely. In one application of this, the VC panner, a common audio signal is fed into both VCA's and one output is sent to the right stereo channel, the other is sent to the left channel. Varying the control voltage moves the sound in stereo space. A crossfader takes two different sound sources and mixes them to a common output. Here, varying the control voltage changes the mix between the two sounds.

##### Tremolo

Tremolo is a periodic rapid wavering of the sound's intensity, similar to vibrato. If your VCA has more than one control input, patch a sinewave LFO with a frequency of around 7-15 hz, with a moderate amplitude into one input and your envelope into another. Or just use the LFO and a steady-state voltage. If your VCA has only one control input then you'll need a DC mixer to combine the control voltages. Using other waveforms such as square or sawtooth for the modulation will yield interestingly different effects.

##### Ring modulation

The VCA and the Ring Modulator are cousins in that a VCA is a two-quadrant signal multiplier and a Ring Modulator is a four-quadrant multiplier. What's that mean? It means that, for a VCA, the output is the instantaneous product of the input signal and the control signal, where the control signal goes to a minimum of zero volts. If you take the control voltage into negative territory it's treated the same as zero. The two quadrants are the top and bottom right quadrants of a Cartesian grid, where positive and negative values are allowed for the audio input but only positive values are allowed for the control input. A Ring Modulator, on the other hand, allows positive and negative values for both control and audio (they're usually called "carrier" and "signal"). When the control goes negative it inverts the audio signal (swaps positive for negative). Just like in math, multiply 1 by -1, get -1, multiply -1 by -1, get 1.

Here's some more math: A ring modulator's output frequency content is the sum and difference of the input frequencies. If you call one input 'A' and the other one 'B' then the output is A+B and A-B the "sum and difference" frequencies are present and the original frequencies are suppressed. A VCA's output will be A+B and A-B and A and B; the original frequencies will be present in the signal along with the sum and difference frequencies.

Ok, what's that mean for your sound? If you want to do ring modulator effects but don't have a ring modulator you can do similar effects with a VCA. Patch audio frequency signals into both audio and control inputs, try different waveforms and different frequencies.

##### Faking it

You can use other modules in place of the VCA to do the traditional job of gating audio, in case your VCA is busted, needs a rest, or is already in use. A VC Lowpass filter is a great candidate for doing this. Keep in mind that in order for this to work the VCF's initial cutoff frequency should be at its lowest, much lower than your audio signal. It's simplest and cleanest at low resonance levels on audio with a low harmonic content, and more interestingly organic or acoustically imitative with more harmonics.

If you have a VC slew limiter this can be used the same general way as the VC LPF. Keep in mind that a slew limiter is a DC-coupled lowpass filter with a fairly gentle roll-off curve. Set the slew limiter's rate (slew speed) at a minimum to attenuate an input sound, use voltage control to increase the slew rate to increase your sound's loudness.

Another VCA stand-in is the Ring Modulator. On a theoretically perfect Ring Modulator it shouldn't matter which of the inputs you use for audio and which for control, they would be interchangeable. However, many real-world designs optimize signal and carrier inputs, so you might want to experiment with which input is good for audio and which is for control. If the Ring Modulator doesn't have DC coupled inputs then long envelopes will be a problem but you may be able to manage short percussive ones. PAIA's old 4700 series modules didn't include a VCA, they used a Ring Modulator with DC inputs.

##### Transient Shapes

How flexible is your system? Envelopes can be messed with in different ways and combinations. The mainstay setup of an exponential VCA and linear envelope most accurately imitates a variety of acoustical instruments, but what if you're looking for something weird? Using a linear VCA and envelope yields somewhat "flat" sounds. An exponential VCA and envelope gives strangely sharp or spikey effects.

A linear VCA and log envelope can sound squashed or murky. Most envelope generators don't provide more than one kind of envelope slope, but if it happens to be a voltage controlled envelope generator, feeding the output back into the vc input with some kind of control in the middle (like a pot) will yield exponential envelopes, and, with an inverted signal, provide log envelopes. Experimenting with combinations of VCA types and envelope shapes offers many surprising possibilities.

##### Interpatch VCA's

VCA's can be used at intermediate stages in a patch to add complexity and flexibility to a sound. As I said earlier, DC coupled linear VCA's are particularly handy for modulating control voltages. Audio VCA's can be used to add brief transients, such as a xylophone's hammer noise or flute 'tonguing', mixed along with the main sound. If you're using multiple VCA's this way keep in mind you'll need a like number of envelopers to drive them and a mixer to combine the various sounds together.

Interpatch VCA's can also be handy in feedback loops, modulating, say, the resonance of a filter or phase shifter.

##### VC mixing

Those lucky enough to have several VCA's at their disposal can do voltage-controlled mixing to produce especially complex sounds before recording or to automate mix-downs using sequencers, MIDI, or other control sources. Serge offers both stereo and quad multichannel VC mixers, where the customer specifies the number of input channels. 








