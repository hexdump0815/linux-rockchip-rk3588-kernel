the following commands were used to extract the boot blocks from the armbian
image from https://www.armbian.com/rock-5b/

xzcat Armbian_22.11.2_Rock-5b_jammy_legacy_5.10.110_xfce_desktop.img.xz | dd of=boot-rock-5b.dd bs=512 seek=1 skip=1 count=32767 status=progress
