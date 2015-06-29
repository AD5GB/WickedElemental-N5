obj-$(CONFIG_F2FS_FS) += f2fs.o
## RDD - dangerous hacks
HOST_CFLAGS += -Wno-array-bounds
KBUILD_CFLAGS += -Wno-array-bounds
CFLAGS_KERNEL += -Wno-array-bounds
CFLAGS_MODULE += -Wno-array-bounds

f2fs-y		:= dir.o file.o inode.o namei.o hash.o super.o inline.o
f2fs-y		+= checkpoint.o gc.o data.o node.o segment.o recovery.o
f2fs-$(CONFIG_F2FS_STAT_FS) += debug.o
f2fs-$(CONFIG_F2FS_FS_XATTR) += xattr.o
f2fs-$(CONFIG_F2FS_FS_POSIX_ACL) += acl.o
