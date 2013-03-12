---
title: 'Progress on Bart&#8217;s Slider'
author: Duane Johnson
layout: post
permalink: /2012/12/progress-on-barts-slider/
categories:
  - Uncategorized
tags:
  - 3D printer
  - buildlog
  - camera slider
  - motorized
---
# 

Today I built out most of the hardware for [Bart’s camera slider][1]. His design uses a moving motor–the motor is attached to a plate that connects orthogonally to the aluminum carriage. The motor then moves itself along a neoprene belt that runs the length of the camera slider.

 [1]: http://www.buildlog.net/wiki/doku.php?id=ms:ms_slider

I made customized some of the parts from my MakerSlider v.0.3 (such as the endcaps) and adjusted them to hold the neoprene belt. Also custom designed is the subplate that Bart originally used a laser cutter to build. Since I have only a 3D printer at the moment, I need to use whatever I have available. And it’s so fun to make things in 3D anyway ![:)][2] 

 [2]: http://makerslider.com/wp/wp-includes/images/smilies/icon_smile.gif

![][3] 
![][4] 
![][5] 
![][6] 

The 3 custom parts are available on github:

 [3]: https://www.dropbox.com/s/dav4see6xj288xi/2012-12-15-neoprene-assembled.jpg?dl=1
 [4]: https://www.dropbox.com/s/vk4no48eozkjpih/2012-12-15-neoprene-carriage.jpg?dl=1
 [5]: https://www.dropbox.com/s/dve8h0m2x65s1o0/2012-12-15-neoprene-carriage-bottom.jpg?dl=1
 [6]: https://www.dropbox.com/s/3y97u91bksxcyjg/2012-12-15-neoprene-endcaps.jpg?dl=1

Subplate

[subplate.scad][7]

Endcap

[endcap.scad][8]

Slotted Neoprene “Washer”

[slotted\_neoprene\_washer.scad][9]

 [7]: https://github.com/canadaduane/MakerSlider/blob/bartslider/subplate.scad
 [8]: https://github.com/canadaduane/MakerSlider/blob/bartslider/endcap.scad
 [9]: https://github.com/canadaduane/MakerSlider/blob/bartslider/slotted_neoprene_washer.scad