the following commands were used to extract the boot blocks from the armbian
image from https://www.armbian.com/orangepi-5/

xzcat Armbian_23.02.0-trunk.0112_Orangepi5_bullseye_legacy_5.10.110.img.xz | dd of=boot-orange-pip-5.dd bs=512 seek=1 skip=1 count=32767 status=progress
