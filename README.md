# latitude e6430 with nvidia dgpu data
So I picked up my favorite model of laptop, the Dell Latitude e6430, with the full intention of flashing libreboot to it. I neglected to consider that there is an NVIDIA dGPU variant of this laptop, which is not supported in Libreboot. Perhaps to be expected, booting did not work. This repository contains autoport output as well as boot logs. You can also find a copy of the original ROM backed up here as well.

Current status: failing to boot. Built with BOOT_DEVICE_SPI_FLASH_NO_EARLY_WRITES enabled based on https://www.mail-archive.com/coreboot@coreboot.org/msg56284.html. Still fails to boot, but cleared error message about MRC cache. Now simply terminates after ram init. Have swapped in multiple RAM modules, tried the RAM in different configs. The original RAM works fine.

I do have a Latitude e6430 iGPU variant which is not really usable (missing too many case pieces, etc) that I was able to flash Libreboot to, so I know I have the basic process correct.

Accepting recommendations/suggestions. :)
