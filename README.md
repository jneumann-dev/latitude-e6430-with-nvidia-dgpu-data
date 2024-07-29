# latitude-e6430-with-nvidia-dgpu-data
So I picked up my favorite model of Dell Latitude e6430, with the full intention of flashing libreboot to it. I figured, how hard can it be? I simply pick up a Raspberry Pi Pico, wire it up to an SOIC-8 clip, flash a custom firmware to it, and start dumping and rewriting the system firmware! _What could possibly go wrong?_

I neglected to consider that, although every e6430 unit I've worked with or randomly picked up has always been the Intel iGPU variant, there _are_ units out there with an NVIDIA dGPU. Now I have a testbed for collecting data/messing around with Libreboot! I am dumping the outputs of various commands I've been asked to run by Libreboot/coreboot developers here. You can also find a copy of the original ROM backed up here.
