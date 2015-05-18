#
# Makefile for the Linux fat filesystem support.
#

# RDD - HACKS!
HOST_CFLAGS += -Wno-array-bounds
KBUILD_CFLAGS += -Wno-array-bounds
CFLAGS_KERNEL += -Wno-array-bounds
CFLAGS_MODULE += -Wno-array-bounds
obj-$(CONFIG_FAT_FS) += fat.o
obj-$(CONFIG_VFAT_FS) += vfat.o
obj-$(CONFIG_MSDOS_FS) += msdos.o

fat-y := cache.o dir.o fatent.o file.o inode.o misc.o
vfat-y := namei_vfat.o
msdos-y := namei_msdos.o
