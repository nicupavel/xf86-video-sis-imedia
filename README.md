# SIS 662/670/671 XOrg driver

Driver for SIS 671 found in Intel D201GLY, it fixes high resolution problems, adds 2D hardware acceleration and XV/XVMC support. 
It requires a kernel patch to add SIS 671 PCI ids (0x0671) and a new entry on sis-agp.c to detect the chipset, see [kernel-patch](kernel-patch/ folder.
This driver only works and compiles on Xorg >= 7.0 versions and has been tested with iMedia Linux on Intel D201GLY mini-itx mainboard.
This driver is derived from the work of Thomas Winischhofer  <thomas@winischhofer.net> on Xorg SIS driver.

## Building

To compile run ./autogen.sh , configure with your desired prefix and make install.

## Maintenance

This driver has already been included in most distributions. See [rpmfind](https://rpmfind.net/linux/rpm2html/search.php?query=x11-driver-video-sisimedia) for 
up to date packages.

