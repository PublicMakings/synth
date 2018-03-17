## Components
* [555 timer, maybe?](http://www.ti.com/lit/ds/symlink/lm555.pdf)
* [cd4040 divider/counter](http://datasheet.octopart.com/CD4040BE-Texas-Instruments-datasheet-7283420.pdf)
* [cd4051 multiplexer/demultiplexer](http://www.ti.com/lit/ds/symlink/cd4051b.pdf)
* [cd40106 - hex schmidt trigger/inverter](http://www.ti.com/lit/ds/symlink/cd40106b.pdf)
* [LM386 audio amp](http://www.ti.com/lit/ds/symlink/lm386.pdf)
* capacitors
* potentiometer
  * 8 x 100k
  * 1 x 10k
  * misc...?
* resistors
* switches
  * on-off-on rocker
  * mom-off-mom rocker
  * on/off slider
  * single pole single throw(is this the right name?)
  * *buttons: both locking buttons and momentary would be useful.*
* LEDS
  * indivual lights for steps
  * ON indicator 
* power supply
  * 9v battery
  * power regulator
* speaker with 1/8" plug?, this would allow for switching with exciter and other output devices

## Core Elements
### General Outline for tones and sequencer
* [Casper Electronics](https://www.youtube.com/watch?v=FaoJaLmZaL4) tutorials!!!
* [good construction notes](https://www.youtube.com/watch?v=x2Jt1os23UM)
* [good usage of reset pin](https://www.youtube.com/watch?v=qI5WTshUXbg)

This [article](http://electro-music.com/forum/phpbb-files/booleansequencertutorial_158.txt) offers a lot of voacb and a conceptual outline which is useful.

Here's a [concrete schematic and simple breakdown](http://little-scale.blogspot.com/2007/06/simple-sequencer.html) of the 40106, 4040, and 4051 combo.

[Similar breakdown](https://jakobglock.wordpress.com/tag/cd4040/), but 555 as oscilator.

More detailed breakdown of [4051](https://hackaday.com/2015/02/23/logic-noise-the-switching-sequencer/).

#### *Controls*
* On/off
* Volume
* Rate
* Step Controls
  * Start/Stop stepper
  * single step
  * potentiometers on the steps
  * momentary switches to play
  * on/off switches
  * toggle for capacitance values? perhaps have only a couple either in groups or in single sections
  * fucked up logic controls jumblers that throws off the binary infeed on the multiplexer, perhaps only momentary switches.


#### *Exapnsion Under the Hood*
have two hex schmidt triggers to allow some breathing room on the tones oscilators; For each inverter have a pair of headers solder in, to allow for additional re-wiring. Also have a selection of resistor values and a few unused pots to add as the bridges. *important to leave room for jumpers, perhaps this section has it's own little opening and board section.



### AMP
* [Basic amp plan video](https://www.youtube.com/watch?v=ZOuZWE_tfgQ) Potentially build this as a seperate board, I can solder up both the bass boost version and the simple one. Have this connect via a jumper and headers for swaping out?
  * have a disconnectable jumper for the gain. 
  * have an additional input for playing through other signals{perhaps a wired pickup?} have a pot on this to regulate the strenght of this signal
  * two outputs, feedback loop?

* [Slightly more complicated amp build](https://www.youtube.com/watch?v=eikfRF66hRA)



### Background Research - Core Concepts
* [capicator conversion chart](http://www.radio-electronics.com/info/formulae/capacitance/capacitor-conversion-chart.php)
  * get an image and paste in!
* [Sampler with Arduino Mega](https://www.youtube.com/watch?v=tUapZ_JdHLE)
* [Class D Amps](https://www.youtube.com/watch?v=O1UagNkcxi4)
* [All about inductors tutorial video](https://www.youtube.com/watch?v=NgwXkUt3XxQ)

### more synth videos & links
* [DIY synth zine](https://www.techwillsaveus.com/az/wp-content/uploads/2014/02/Synth_manual_V2.0_digital.pdf)
*
* [Basement drum machine genius](https://www.youtube.com/watch?v=bPvnk-ShM8E)
* [LFO to 40106 ocilator](https://www.youtube.com/watch?v=2iBgvQXzvTA)
* [QUICK Build video](https://www.youtube.com/watch?v=RfKNHV9t8so)
* [Lot of good schematics](http://musicfromouterspace.com/analogsynth_new/SEQ16_2006/SEQ16_2006.php), a sight worth revisiting.
* 
* [Sweet and funny cardboard bo build](http://www.instructables.com/id/10-Step-Analog-Sequencer/) 
*
* [no talking, but a couple crucial schematics](https://www.youtube.com/watch?v=LNHLZY0Hvqk)
* [Polyphonic tone generator](https://www.youtube.com/watch?v=LFyvaDnOTBw) ** __worth exploring more__
* [3d print](http://blog.tommy.sh/posts/okay-synth)
* [casper electronics triggering with transistors](https://web.archive.org/web/20161126125254/http://casperelectronics.com/finished-pieces/circuit-bending-tutorial/looping-with-transistors/)
* [useful 'splaining going on](https://www.youtube.com/watch?v=f9GO3OC8oDY) **
* [Electro Music](http://electro-music.com/) seems like the site is no longer maintained, but useful articles.
* [Grumpy guy with lots of modules](https://www.cgs.synth.net/modules/) 


