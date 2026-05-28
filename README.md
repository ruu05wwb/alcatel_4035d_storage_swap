# alcatel_4035d_storage_swap
Recovering Alcatel POP3 4035D (MTK6572) with dead eMMC by migrating OS to the Micro-SD card 

Background. The device has switched off while charging. After that it was only able to show the initial logo and then looping into reboots, or enter recovery.

The standard flash attepmts (like in the below vieo) didn't help. CTR recovery logs were showing lack of "mmcblk0p5-mmcblk0p9", and ADB - I/O errors in the remaining partitions excepting for "mmcblk0boot0-mmcblk0boot1" which indicated physical corruption of the main part of eMMC.

Hence was decided to move sytem, and other partitions to the Micro-SD. This was successfully dome  now the device is fully operational.

Folders "boot" and "recovery contain only the files which have been changed in the project, preserving the folder structure.

Sources which were used as a base for modifications:
- boot: backup from here https://disk.yandex.ru/d/oAyMeG3YIKYKbg (referenced in the video https://www.youtube.com/watch?v=3sH75eHLuNs)
- recovery: CTR recovery https://4pda.to/forum/index.php?showtopic=625531&st=1040#entry56868570