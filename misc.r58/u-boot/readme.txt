the following commands were used to extract the boot blocks from the armbian
images from https://www.armbian.com/rock-5b/ and https://www.armbian.com/orangepi-5/

xzcat Armbian_22.11.2_Rock-5b_jammy_legacy_5.10.110_xfce_desktop.img.xz | dd of=boot-rock-5b.dd bs=512 seek=1 skip=1 count=32767 status=progress
xzcat Armbian_23.02.0-trunk.0112_Orangepi5_bullseye_legacy_5.10.110.img.xz | dd of=boot-orange-pip-5.dd bs=512 seek=1 skip=1 count=32767 status=progress
