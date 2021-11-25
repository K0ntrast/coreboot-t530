Precompiled EC patches for th Lenovo T530. Credits to Hamish Coleman's EC patch for xx30 series Thinkpads.
https://github.com/hamishcoleman/thinkpad-ec

Image: Battery Patch Applied: Keyboard Patch Applied:
[t530-2.75-1.13-nokb-bat.img] N Y
[t530-2.75-1.13-nokb-nobat.img] N N
[t530-2.75-1.13-kb-bat.img] Y Y
[t530-2.75-1.13-kb-nobat.img] Y N

Following the build instructions here:
https://bystram.be/posts/thinkpad-x230-battery-ec-patch/

Decompress the archive and use this command to write it to USB:

  sudo dd if=[imagename.img] of=/dev/[usbdrive] bs=4M status=progress conv=fsync

Boot to the USB drive and apply the patch.

AC adapter and battery must be present for the upgrade to work.
