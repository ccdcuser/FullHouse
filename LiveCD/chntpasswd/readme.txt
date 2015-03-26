How to make the CD

Unzipped, there should be an ISO image file (cd??????.iso). This can be burned to CD using whatever burner program you like, most support writing ISO-images. Often double-clikcing on it in explorer will pop up the program offering to write the image to CD. Once written the CD should only contain some files like "initrd.gz", "vmlinuz" and some others. If it contains the image file "cd??????.iso" you didn't burn the image but instead added the file to a CD. I cannot help with this, please consult you CD-software manual or friends.

The CD will boot with most BIOSes, see your manual on how to set it to boot from CD. Some will auto-boot when a CD is in the drive, some others will show a boot-menu when you press ESC or F10/F12 when it probes the disks, some may need to have the boot order adjusted in setup.

How to make an bootable USB drive

Copy all the files that is inside the usbXXXXXX.zip or on the CD onto an usb drive, directly on the drive, not inside any directory/folder.
It is OK if there are other files on the USB drive from before, they will not be removed.
Install bootloader on the USB drive, from command prompt in windows (start the command line with "run as administrator" if possible)
X:syslinux.exe -ma X:
Replace X: with the drive letter the USB drive shows up as (DO NOT USE C:)
If it seems like nothing happened, it is usually done.
However, a file named ldlinux.sys may appear on the USB drive, that is normal.
It should now in theory be bootable.
Please know that getting some computers to boot from USB is worse than from CD, you may have to change settings, or some will not simply work at all.