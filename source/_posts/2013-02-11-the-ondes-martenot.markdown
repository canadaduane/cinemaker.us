---
title: The Ondes Martenot
author: Duane Johnson
layout: post
permalink: /2013/02/the-ondes-martenot/
categories:
  - Hardware
  - Design
---

![][1]

 [1]: /images/2013-02/ondes-martenot.jpg

I’ve been racking my brains for the past couple of weeks trying to figure out a way to make a "sliding potentiometer" the full length of the cinemaker pocket dolly. Today, after one lucky email exchange, I have a cost effective solution that sounds like music to my ears.

In frustration with my expensive or otherwise difficult-to-implement ideas, I sent the following email to my friends back in the Chicago hackerspace (PS1):

> I want to be able to measure the distance from one end of an aluminum extrusion to two (variable) points along the length of the extrusion. e.g.
>
>
>
>  
> |====================aluminum======================| 1 meter  
> sensor>           [knob]            [knob]
>
>
> 
>
> Basically, I want to recreate the functionality of a double "slide potentiometer" but the slide is 1m long. Each of the "[knob]" things in the above blueprint is a knob that can slide the entire length of the aluminum extrusion.
> 
> I’ve considered many options for the sensor. Some measure relative distance (e.g. an optical mouse sensor that reads "tick" marks along the bottom, or a "spring-loaded" coil of string with a rotary encoder on the coil) and some measure absolute distance (e.g. an infrared sensor, an ultrasonic sensor, or a video camera). After giving it some thought, I think only the absolute distance measurements will work in this case, since I can’t know where the starting location of the knobs when the system is powered on.
> 
> The cheapest method seems to be ultrasonic sensors (see [1]), however I don’t want wires dangling. One way to avoid power and wires to the knobs is if I mount one tranceiver on the end of the aluminum extrusion (as pictured above). However, then the problem is that the sensor detects the BAR ITSELF and says "hey something is really close". I could get around this by mounting 2 more ultrasonic tranceivers–one at each of the sliding knobs I want to measure. In this scenario, instead of sending and receiving the ultrasonic pulse from the same location, I could break it up and send at the knob and receive at the end of the aluminum extrusion. If I take this course, however, it means I must send power through wires to ultrasonic transmitters at the knobs.
> 
> Again, I don’t want wires hanging about. So I was thinking, as a software engineer is generally wont to do, about computer vision. I could hypothetically mount a camera at one end of the slider (as pictured) and then look for "hot pink" colored knobs. Divide the inverse ratio of non-hot-pink pixels to hot-pink pixels and I would get the absolute  
> distance to the hot pink knobs. This method could work since "hot pink" is not generally found in natural environments (except for my 3 year old daughter’s birthday party…) 
> 
> The problem with the above solution is that video cameras are a little more expensive than ultrasonic sensors, and much more computationally intensive. So that got me thinking. What if I could coat the knobs with a material that is the "sonic equivalent" of hot pink? Does such a thing exist? Is there a way to detect echoes from various surfaces such that the receiver will ignore certain types of (non-hot-pink) sounds?
> 
> I know it’s kind of a crazy analogy, but since I’ve hit a wall with ideas I thought I’d ask for your thoughts. If anyone has any ideas I’d love to hear them.

Mason replied:

> Dare I ask why you wouldn’t use something like what an Ondes Martinot http://en.wikipedia.org/wiki/Ondes_Martenot uses? It seems pretty darn close to "slide potentiometer" in actual function, with the length you desire.

"The Ondes Martenot? What the heck is that?" I thought. It turns out that there’s a beautiful instrument invented in the early 20th century that uses a "ring" (the kind of ring you put your finger in) to slide along the length of a keyboard/piano. The position of the ring indicates the pitch of the musical sound. If you’ve ever heard 1950s style "eerie martian music" it was probably an Ondes Martenot.

Shocked and amazed, I went to the wikipedia page to try to figure out how it works. Unfortunately, the technical details were scant. So I turned to google and sure enough, someone has re-created the Ondes Martenot and revealed its secret! Dana Countryman gave this demonstration of his DIY instrument:

So the take-away for me is this: keep the creative ideas flowing, but don’t hesitate to go to a group of knowledgeable people with a seemingly intractable problem–they are bound to drop an OMG why didn’t I think of that? bomb and make life simpler.