# latitude e6430 with nvidia dgpu data
So I picked up my favorite model of laptop, the Dell Latitude e6430, with the full intention of flashing libreboot to it. I figured, how hard can it be? I simply pick up a Raspberry Pi Pico, wire it up to an SOIC-8 clip, flash a custom firmware to it, and start dumping and rewriting the system firmware! _What could possibly go wrong?_

I neglected to consider that, although every e6430 unit I've worked with or randomly picked up has always been the Intel iGPU variant, there _are_ units out there with an NVIDIA dGPU. Perhaps to be expected, booting did not work. Now I have a testbed for collecting data/messing around with Libreboot, at least until I get tired of messing with it and flip it! I am dumping the output of autoport as well as boot logs here. You can also find a copy of the original ROM backed up here.

Current roadblock is that the MRC cache fails 

> Transaction timeout between offset 0x00031683 and 0x00031684 (= 0x00031683 + 1) HSFC=1804 HSFS=6000!
> SF: write failure at 40000
> REGF metadata allocation failed: 101 data blocks 4096 total blocks
> MRC: failed to update 'RW_MRC_CACHE'.
> CBMEM entry for DIMM info: 0x7ffdb000
