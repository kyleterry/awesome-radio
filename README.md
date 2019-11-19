# Awesome Radio [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome radio resources. Inspired by awesome-*.

This project is aimed at hackers who enjoy all aspects of radio communication.
While a lot of this technology isn't usable by citizens and is heavily regulated
by the FCC, just knowing anything about it is special. I've been interested in
learning the ins and outs of radio, as well as hearing stories, new and old.

You can find some information at [wiki](../../wiki).

Software Defined Radio is a way to define components that are typically
hardware, such as filters and amplifiers, as software. It has been around for a
while, but with the cost of digital electronics needed to run SDR becoming
increasingly cheaper, we are seeing a rise in hacker folk playing and building
with SDR.

I would like contributors for this section.

## Hardware
* __Recommended starter hardware__ On the low end,
  [RTL-SDR](http://sdr.osmocom.org/trac/wiki/rtl-sdr) is a super-cheap usb
  dongle, around which a thriving community has been founded.
* On the other side of the cost spectrum, [pervices](http://www.pervices.com/)
  makes some really high-throughput, PCIe devices for when you need to log all
  the traffic ever. The software and community support for this is less good,
  though (for which you can blame @outofculture).
* You can also browse through the [big
  list](https://gnuradio.org/redmine/projects/gnuradio/wiki/Hardware) of all
  compatible hardware.
* Antennas are their own body of options and tradeoffs, about which I know
  nothing.
  
### Links
* [Portable SDR](http://hackaday.io/project/1538-PortableSDR)

## Software
Depending on the hardware you're using, it may ship with some demo software to
play around with. This is great for just getting a chance to see some waves and
start to get an idea of what's possible. Otherwise, [GNU
Radio](https://gnuradio.org/redmine/) is going to where you'll spend your time.
It's mainly just a library, but it also has a supporting gui for combining
processing blocks that then outputs python. Once you're more comfortable, you
can also just use GNURadio to do any device tuning, setup and i/o, and then use
numpy for the signal manipulation math.

Just visualizing and manually inspecting a signal is a valuable part of learning
how to work with them. [Baudline](http://www.baudline.com/) is a janky old
thing, but it's the best there is. Be forewarned that learning the UI won't come
easily to anyone.

### Links

* [Gqrx](http://gqrx.dk/)
* [sdrsharp on .NET](http://sdrsharp.com)
* [some gr sketches](https://github.com/evan-schaffer/GNURadioSDR)
* [Shinysdr project](https://github.com/kpreid/shinysdr)
* [UHF RFID reader for lime](https://github.com/DasSidG/limesdr_rfid)
* [SDR Educational Tools For Raspberry Pi](https://github.com/myriadrf/ScratchRadio)
* [Oscilloscope tool](https://github.com/analogdevicesinc/scopy)
* [audio filter for GR](https://github.com/ntoulasd/DSP)
* [Interesting encoders/decoders for GR](https://github.com/mberntsen/gnuradio-plugins)
* [ACARS decoders](https://github.com/mmmaaaxxx/SUPACARS)
* [Cool phosphor spectrum](http://osmocom.org/projects/sdr/wiki/fosphor)
* [example for gr-fosphor](https://github.com/g0hww/qtrfiq)
* [goTenna Mesh](https://github.com/argilo/gr-tenna)
* [M100 DJI controlling](https://github.com/sunytux/GnuRadio-DJI_channel)
* [RF transmitter for Raspberry Pi (only GPIO needed)](https://github.com/F5OEO/rpitx)


#### Keyless remote

* [Remote keyless, include good paper](https://github.com/tharina/RKE)
* [Jamming and replay RKE](https://github.com/darvarr/jamming-and-replay)

#### GPS

* [GPS simulation](https://github.com/emlyons2014/gps-sim)
* [Software correlator for GPS](https://github.com/psas/gps)
* [http://sdrgps.blogspot.com](https://github.com/hahnpv/sdrgps)
* [SDR GPS receiver](https://github.com/ajinkyagorad/GPSrx)
* [GPS simulation](https://github.com/ookk2011/GNSS-GPS-SDR)

## Public Health and Safety

Police and fire in the United States typically communicate over trunked radio.
This makes it hard to scan using normal reciever without trunk tracking
abilities. See more in the [trunking](#trunking) section.

### Trunking

While not strictly specific to public health and safety, it is usually the first
thing that comes to mind when talking about trunked radio.

Trunked radio is a form of digital-two-way communication where multiple
organizations can share a small spectrum of real frequencies without hearing
another organizations conversations. A user can choose a logical channel or
group and the base station will find an empty frequency to transmit on.

### Links

* [Project 25](http://www.project25.org/)
* [Project 25 wikipedia](http://en.wikipedia.org/wiki/Project_25)
* [Trunked Radio wikipedia](http://en.wikipedia.org/wiki/Trunked_radio_system)
