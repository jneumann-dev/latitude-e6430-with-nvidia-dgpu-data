# latitude e6430 with nvidia dgpu data
So I picked up my favorite model of laptop, the Dell Latitude e6430, with the full intention of flashing libreboot to it. I figured, how hard can it be? I simply pick up a Raspberry Pi Pico, wire it up to an SOIC-8 clip, flash a custom firmware to it, and start dumping and rewriting the system firmware! _What could possibly go wrong?_

I neglected to consider that, although every e6430 unit I've worked with or randomly picked up over the years has always, by chance, been the Intel iGPU variant, there _are_ units out there with an NVIDIA dGPU. Just my luck that the one I order with the intent to libreboot is the rarer, unsupported NVIDIA variant. Perhaps to be expected, booting did not work. This repository contains autoport output as well as boot logs. You can also find a copy of the original ROM backed up here as well.

Current status: failing to boot. Built with BOOT_DEVICE_SPI_FLASH_NO_EARLY_WRITES enabled based on https://www.mail-archive.com/coreboot@coreboot.org/msg56284.html. Still fails to boot, but cleared error message about MRC cache. Now simply terminates after ram init. Unsure how to proceed.
