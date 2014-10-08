88W8764-firmware
================
Starting at offset 0, there is a 16 byte header.  This header repeats every 512 bytes.  It is of the form:  
0100 0000 XXXX XXXX 0002 0000 XXXX XXXX

Seems like an artifact of flash devices, but the mwl8k driver uses the 0100 bytes to verify that this is 88W8764 firmware.

This firmware was released as C headers found in mrvl_wlan_v7drv.  Reference design drivers that were released as a part of Linksys' firmware GPL tarball for the WRT1900AC.  I just put the bytes together.
