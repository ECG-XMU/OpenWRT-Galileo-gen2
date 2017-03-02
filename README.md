OpenWRT-Galileo-gen2
===============

OpenWRT for Intel Galileo Gen 2

OpenWRT version: git-svn-id: svn://svn.openwrt.org/openwrt/trunk@42607

Intel® Galileo Board Toolchain: https://downloadcenter.intel.com/download/24619/Intel-Galileo-Board-Toolchain

How to Build?

running "make V=99 " to build the OpenWRT firmware for Intel Galileo. When build finished, the kernel image and cross-compiler can be found in the following directory:

The kernel image: " /../build_dir/target-i386_i486_uClibc-0.9.33.2/linux-x86_galileo "

The cross-compiler: " /../staging_dir/toolchain-i386_i486_gcc-4.8-linaro_uClibc-0.9.33.2/"

How to use?

put the following files to your tf card:

/boot/grub/grub.conf

/bzImage

/grub.efi

/openwrt-x86-galileo-rootfs.cpio.gz

Note:

（1）”bzImage” is in the directory of "build_dir/target-i386_i486_uClibc-0.9.33.2/linux-x86_galileo"

（2） the root filesystem "openwrt-x86-galileo-rootfs.cpio.gz" is in the directory of "bin/x86"

（3）"boot" and "grub.efi"  download from the github  https://github.com/ECG-XMU/SDcard_grub.git

