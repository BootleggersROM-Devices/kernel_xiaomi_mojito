#
# Makefile for the Linux eCryptfs
#

obj-$(CONFIG_ECRYPT_FS) += ecryptfs.o

ecryptfs-y := dentry.o file.o inode.o main.o super.o mmap.o read_write.o \
	      crypto.o keystore.o kthread.o

ifdef CONFIG_DEBUG_KERNEL
ecryptfs-y += debug.o
endif

ecryptfs-$(CONFIG_ECRYPT_FS_MESSAGING) += messaging.o miscdev.o
