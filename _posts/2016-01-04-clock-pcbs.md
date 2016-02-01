---
layout: post
title: Incandescent Clock PCBs
tags: electronics projects pcb
published: true
---

I'm in the process of making a large digital clock out of [tubular incandescent bulbs](https://www.1000bulbs.com/product/5764/IN-S3280.html). I designed my own power circuitry for this clock, because it is a cheaper and more reliable option than what is available. I don't trust the crude results of a PCB mill with high voltages, so I decided to try out [DirtyPCBs](http://dirtypcbs.com/).

## Quad Relay

Each board contains four relays, which can be directly or serially controlled. The 4-bit latching shift register allows the boards to be daisy chained. Each relay slot can be occupied by either a mechanical or solid state relay in the same footprint.

![image](/media/2016-01-04-clock-pcbs/relay-sch.png)

![image](/media/2016-01-04-clock-pcbs/relay-brd.png)

## AC Dimmer

The dimmer emits a "zero-crossing" pulse for each time the input sine wave crosses zero volts (ex. 120Hz in US). By delimiting the waveform, the circuits allows a microcontroller to control the connected AC load by powering it for a portion of each sine period. The duty cycle corresponds (non-linearly) to the dimming intensity.

![image](/media/2016-01-04-clock-pcbs/dimmer-sch.png)

![image](/media/2016-01-04-clock-pcbs/dimmer-brd.png)
